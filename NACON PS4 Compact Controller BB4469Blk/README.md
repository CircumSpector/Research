# NACON PS4 Compact Controller BB4469Blk

## Highlights

When connected to a Windows PC it represents itself as an XUSB-compatible Xbox 360 Controller. By default, it manages to stall/freeze tools like USB Tree View and Wireshark/USBPcap due to some jet unidentified firmware problem.

We're basically trying to figure out if we can use this controller in "PS4 mode" on PC instead of XUSB (which it currently represents itself) to get all features like touch inputs etc. to feed it into DS4Windows or similar tools.

My particular model can be switched to WinUSB using Identinator and the `winusb.reg` file in this folder. It will not work via GUI due to a bug.
