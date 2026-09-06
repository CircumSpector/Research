# Research

Research & Development Resources regarding Gaming Input Peripherals.

## About

An ever growing collection of research material, firmware copies, packet dumps and documentation about PS4/PS5/Xbox/... controllers that could potentially be used on PC via DS4Windows, \[REDACTED\]Bus and alike.

## Tools

- [USB Descriptor and Request Parser](http://eleccelerator.com/usbdescreqparser/)
- [Wireshark](https://www.wireshark.org/)
- [USB Device Tree Viewer](https://www.uwe-sieber.de/usbtreeview_e.html)

## How you can help

You do not need to be a programmer or reverse engineer to contribute. If you have a controller that is missing here, or a capture of a scenario we do not have yet, a careful Windows USB recording plus a short write-up is already useful.

This page walks through:

1. What files and notes to collect
2. How to record USB traffic on Windows with Wireshark
3. How to describe the device so someone else can use the capture
4. How to send the files with GitHub Desktop and open a pull request

The capture steps below are for **Windows USB** traffic. Bluetooth and Linux captures are welcome too, but they are not covered here.

## What to send

Useful submissions usually include some mix of the following:

| Item | Why it helps |
| --- | --- |
| USB packet capture (`.pcapng`) | Shows what the controller and Windows actually exchange |
| Short notes about the device and the exact steps you took | Makes the capture usable instead of a mystery file |
| USB Device Tree Viewer report | Identifies vendor ID, product ID, revision, and how Windows sees the device |
| Photos of the pad, PCB, or labels | Helps match hardware revisions and knockoffs |

You do not have to send everything. A clean plugin capture plus a filled-in device folder is already a good start.

## Safety and privacy

USB capture records traffic for **every device on the same USB host controller**, not only the controller you care about. Treat the resulting file as sensitive.

- Installing USBPcap and capturing USB traffic needs administrator rights. Only install the official Wireshark/USBPcap packages, and reboot when the installer asks.
- Unplug unused USB devices before you start: flash drives, phones, webcams, extra hubs, and wireless dongles. A keyboard and mouse on a different controller is fine; a phone that starts syncing on the same hub is not.
- Captures can include serial numbers and other device identifiers. Photos can include receipts, usernames, or desktop clutter. Review both before you submit.
- Do not share captures from someone else's machine without their permission.
- Save the raw capture. Do not "clean it up" in a hex editor or replace it with a screenshot of Wireshark.

If you are unsure whether a file contains personal information, say so in the pull request and a maintainer can help review it.

## Capture USB traffic on Windows

### 1. Install Wireshark and USBPcap

1. Download Wireshark from [https://www.wireshark.org/](https://www.wireshark.org/).
2. Run the installer.
3. When the installer offers additional components, leave **USBPcap** enabled. This is the Windows USB capture driver. If you already installed Wireshark without it, run the installer again and add USBPcap.
4. Reboot when asked. USBPcap will not show up until after a restart.

USBPcap's own site is [https://desowin.org/usbpcap/](https://desowin.org/usbpcap/). You normally do not need a separate download if Wireshark installed it.

### 2. Confirm USB capture is available

1. Open Wireshark. If no USB interfaces appear, right-click the shortcut and choose **Run as administrator**.
2. On the start screen you should see one or more interfaces named `USBPcap1`, `USBPcap2`, and so on. Each one is a USB host controller (a group of ports), not a single physical port.
3. If those names are missing, USBPcap is not installed or the PC has not been rebooted.

### 3. Find the interface that sees your controller

Wireshark cannot usefully record a controller that is plugged into a different host controller than the one you selected.

1. Leave the game controller **unplugged**.
2. In Wireshark, click the small gear icon next to a `USBPcap` interface if you have one. That options dialog lists devices already on that controller.
3. If you are not sure which interface to use, start a short test capture on `USBPcap1`, plug the controller in, and watch for a burst of USB packets. If nothing new appears, stop, try the next `USBPcap` interface, and repeat.
4. [USB Device Tree Viewer](https://www.uwe-sieber.de/usbtreeview_e.html) can also help: plug the controller in, find it in the tree, and note the hub/port chain. After that, unplug it again before the real capture.

### 4. Record one scenario

Do one job per file. A plugin capture, a firmware-updater capture, and a "play the game for ten minutes" capture should be three files, not one.

1. Unplug the controller. Close other programs that talk to gamepads if you can (Steam Input, DS4Windows, vendor software), unless that software is the thing you are documenting.
2. Start the capture on the correct `USBPcap` interface **before** you plug the device in. The first seconds after connection (enumeration) are often the most useful part.
3. Plug the controller into a **direct motherboard or case port** if you can. Avoid cheap unpowered hubs for the recording.
4. Perform one documented action, for example:
   - Plug in and wait until Windows finishes installing it
   - Switch the pad into another mode (XInput, DirectInput, "PS4 mode", and so on) and plug it in again
   - Hold the vendor's firmware-update button combo while plugging in
   - Press each face button, stick, trigger, and pad once
   - Launch one specific official app or updater and complete one short action
5. Stop the capture as soon as that action is done. Long recordings get large and fill up with unrelated USB noise.
6. Use **File → Save As** and keep the format as **pcapng**.
7. Open the saved file in Wireshark once to confirm it is not empty.

Do not export a CSV, a screenshot, or a "selected packets only" file unless a maintainer asked for that. The original `.pcapng` is the artifact.

### 5. Name the file so it explains itself

Match the style already used in this repository:

```text
2026-09-06_nacon_bb4469_windows_plugin.pcapng
2024-02-23_ds_bth_pairing_capture.pcapng
2023-03-14_logitech_driving_force_gt_plugin_OS_stock_drivers.pcapng
```

A good name includes the date, a short device nickname, and the scenario. Use only letters, numbers, hyphens, and underscores.

### 6. Make the capture worth keeping

- Start recording with the device disconnected so the plugin/enumeration traffic is in the file.
- Keep one scenario per file, and write down the exact button presses or program you used.
- Write down Windows version, controller firmware version if you know it, and any extra software that was running (DS4Windows, Steam, a vendor updater).
- If the pad has several personalities, capture each mode separately and say how you selected that mode.
- After saving, confirm the file opens and that you can see USB packets around the moment you plugged the device in.

## Describe the device

This repository uses **one folder per device**, named after the product people would search for:

```text
Sony DualSense/
NACON PS4 Compact Controller BB4469Blk/
Knockoff PS3 Controller/
```

If the device is already here, add your new capture and notes to that folder. If it is new, create a folder with the manufacturer and model, then put the capture and a `README.md` inside it.

Optional extras that fit the existing layout:

- `images/` for photos
- a `.txt` export from USB Device Tree Viewer
- firmware copies as `.bin` (these are stored with Git LFS, same as `.pcapng`)

### Device README template

Copy this into `README.md` in the device folder and fill in what you know. Empty lines are fine. Guessing is worse than writing "unknown".

```markdown
# Manufacturer Model Name

## Device

- Manufacturer:
- Product name / SKU:
- Hardware revision / date code (if printed on the case or PCB):
- USB vendor ID (VID):
- USB product ID (PID):
- Connection: USB
- Mode during the capture (XInput, DirectInput, PS4, updater, ...):
- Firmware version (if shown by an official app):

## Capture environment

- Windows version (Settings → System → About):
- Other gamepad software running (none / Steam / DS4Windows / vendor app):
- Wireshark version:
- USBPcap installed with Wireshark: yes

## Scenario

What you captured, in order:

1. Started Wireshark on USBPcapN with the controller unplugged
2. ...
3. Stopped the capture

## Files

- `YYYY-MM-DD_device_scenario.pcapng`:
- `UsbTreeView` report or pasted dump:
- Photos:

## Notes

Anything odd: extra modes, button combos, the pad freezing USB Device Tree Viewer, knockoff labeling, and so on.
```

To collect identifiers without extra tools, plug the controller in, open **Device Manager**, find the game controller or USB device, open **Properties → Details**, and choose **Hardware Ids**. You should see something like `USB\VID_054C&PID_0CE6`. The four digits after `VID_` and `PID_` are what to copy.

To collect a descriptor dump, run [USB Device Tree Viewer](https://www.uwe-sieber.de/usbtreeview_e.html), select the controller, and copy the report into the README or save it as a `.txt` file in the same folder.

## Send the files with a pull request

A **pull request** (PR) is a request that this project accept the files from your copy of it. You will:

1. Make a **fork** (your own copy of the project on GitHub)
2. Download that copy with **GitHub Desktop**
3. Add your folder and capture on your PC
4. **Commit** and **push** (save a snapshot, then upload it)
5. Open the pull request on the GitHub website

You need a free [GitHub account](https://github.com/signup).

### Do not upload `.pcapng` in the browser

This repository stores packet captures with [Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage) (Git LFS). The `.pcapng` and `.bin` rules are already in [`.gitattributes`](.gitattributes).

GitHub's **Add file → Upload files** page does **not** store those uploads as LFS objects. A browser upload can produce a commit that looks fine and then breaks clones, or it can fail because the file is larger than the website's 25 MiB limit.

Use GitHub Desktop (or another LFS-aware Git client) to add captures. Use the GitHub website afterward to write the pull request.

### 1. Fork the repository

1. Open [https://github.com/nefarius/GameControllerResearch](https://github.com/nefarius/GameControllerResearch).
2. Sign in.
3. Click **Fork** in the top right and create the fork under your account. Leave **Copy the default branch only** checked unless you have a reason not to.

You now have `https://github.com/YOUR-USERNAME/GameControllerResearch`.

### 2. Install GitHub Desktop and clone your fork

1. Install [GitHub Desktop](https://desktop.github.com/) and sign in with the same GitHub account.
2. In GitHub Desktop: **File → Clone repository**.
3. Select your fork (`YOUR-USERNAME/GameControllerResearch`), choose a local folder, and click **Clone**.

GitHub Desktop includes Git LFS, but you still need to turn it on once on this PC:

1. In GitHub Desktop, open the cloned repository.
2. Choose **Repository → Open in Command Prompt** (or **Open in Git Bash**). If that menu item is missing, choose **Repository → Show in Explorer**, click the folder address bar, type `cmd`, and press Enter.
3. Type the following and press Enter:

```text
git lfs install
```

You should see `Git LFS initialized.` You only need to do this once per computer, not once per contribution.

### 3. Create a branch

A **branch** is a named line of work so your upload is not mixed into `master` until it is reviewed.

1. In GitHub Desktop, click **Current branch**.
2. Click **New branch**.
3. Name it after the device or scenario, for example `add-nacon-bb4469-plugin-capture`.
4. Create the branch from `master`.

### 4. Add your files in File Explorer

1. In GitHub Desktop, choose **Repository → Show in Explorer**.
2. If the device is new, create a folder next to the existing device folders. Use the same naming style (`Manufacturer Model`).
3. Copy your `.pcapng` into that folder. Do not rename it to drop the `.pcapng` extension.
4. Create or update `README.md` with the template above. Notepad is enough. Keep the `.md` extension.
5. Add photos under an `images` folder only if they help identify the hardware.

GitHub Desktop's **Changes** tab should now list the new folder and files.

### 5. Commit and push

1. In GitHub Desktop, keep the new files checked.
2. In **Summary**, write a short description such as `Add USB plugin capture for NACON BB4469`.
3. Click **Commit to** your branch.
4. Click **Push origin** to upload the branch to your fork.

If GitHub Desktop warns that large files need Git LFS, do not skip LFS and do not switch to a browser upload. Confirm LFS is initialized as above and push again.

### 6. Open the pull request on GitHub

1. Open [https://github.com/nefarius/GameControllerResearch](https://github.com/nefarius/GameControllerResearch) (the original project, not only your fork).
2. If GitHub shows a yellow banner **Compare & pull request**, use that.
3. If the banner is gone: click **Pull requests → New pull request**, then **compare across forks**. Set the base repository to `nefarius/GameControllerResearch` and branch `master`. Set the head fork to your copy and the compare branch to the branch you just pushed.
4. Title the request after the device and scenario.
5. In the description, say what you captured, on which Windows version, and how to reproduce the steps. Mention any extra software that was running.
6. Click **Create pull request**.

After that, wait for review. A maintainer may ask for a shorter capture, a missing VID/PID, or a USB Device Tree Viewer dump. You can add files to the same branch in GitHub Desktop, commit, and push; the pull request updates automatically.

## Pre-submission checklist

- [ ] The controller was unplugged when the capture started, then connected on purpose
- [ ] The file is a `.pcapng` saved from Wireshark, and it opens again on your PC
- [ ] One scenario per capture file, with the steps written down
- [ ] Device folder uses the manufacturer/model naming already used here
- [ ] `README.md` includes VID/PID if you can get them, Windows version, and the action sequence
- [ ] Photos and notes were checked for personal information
- [ ] Files were added with GitHub Desktop, not GitHub's browser uploader
- [ ] `git lfs install` was run once on this PC before pushing captures
- [ ] The pull request says what the capture is and how it was made

## Official documentation

- [Wireshark](https://www.wireshark.org/)
- [USBPcap](https://desowin.org/usbpcap/)
- [USB capture setup (Wireshark Wiki)](https://wiki.wireshark.org/CaptureSetup/USB)
- [USB Device Tree Viewer](https://www.uwe-sieber.de/usbtreeview_e.html)
- [GitHub Desktop](https://desktop.github.com/)
- [Git LFS and GitHub Desktop](https://docs.github.com/en/desktop/configuring-and-customizing-github-desktop/about-git-large-file-storage-and-github-desktop)
- [Fork a repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)
- [Creating a pull request from a fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
