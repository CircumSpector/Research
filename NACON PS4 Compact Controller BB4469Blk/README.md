# NACON PS4 Compact Controller BB4469Blk

## Highlights

When connected to a Windows PC it represents itself as an XUSB-compatible Xbox 360 Controller. By default, it manages to stall/freeze tools like USB Tree View and Wireshark/USBPcap due to some jet unidentified firmware problem.

We're basically trying to figure out if we can use this controller in "PS4 mode" on PC instead of XUSB (which it currently represents itself) to get all features like touch inputs etc. to feed it into DS4Windows or similar tools.

My particular model can be switched to WinUSB using [Identinator](https://github.com/nefarius/Identinator) and the `winusb.reg` file in this folder. It will not work via GUI due to a bug.

## "Updater" mode

When `Share` and `Options` buttons are kept pressed simultaneously while plugging it into a PC, the pad seems to switch into some sort of firmware flash mode? The device name changes to "Updater" and uses IDs VID `0x2f24` and PID `0x0001`.

### Wireshark

```text
Frame 2: 46 bytes on wire (368 bits), 46 bytes captured (368 bits) on interface \\.\USBPcap2, id 0
USB URB
DEVICE DESCRIPTOR
    bLength: 18
    bDescriptorType: 0x01 (DEVICE)
    bcdUSB: 0x0110
    bDeviceClass: Device (0x00)
    bDeviceSubClass: 0
    bDeviceProtocol: 0 (Use class code info from Interface Descriptors)
    bMaxPacketSize0: 64
    idVendor: Unknown (0x2f24)
    idProduct: Unknown (0x0001)
    bcdDevice: 0x0120
    iManufacturer: 1
    iProduct: 2
    iSerialNumber: 0
    bNumConfigurations: 1

Frame 4: 37 bytes on wire (296 bits), 37 bytes captured (296 bits) on interface \\.\USBPcap2, id 0
USB URB
CONFIGURATION DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x02 (CONFIGURATION)
    wTotalLength: 34
    bNumInterfaces: 1
    bConfigurationValue: 1
    iConfiguration: 0
    Configuration bmAttributes: 0x80  NOT SELF-POWERED  NO REMOTE-WAKEUP
    bMaxPower: 50  (100mA)

Frame 6: 62 bytes on wire (496 bits), 62 bytes captured (496 bits) on interface \\.\USBPcap2, id 0
USB URB
CONFIGURATION DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x02 (CONFIGURATION)
    wTotalLength: 34
    bNumInterfaces: 1
    bConfigurationValue: 1
    iConfiguration: 0
    Configuration bmAttributes: 0x80  NOT SELF-POWERED  NO REMOTE-WAKEUP
    bMaxPower: 50  (100mA)
INTERFACE DESCRIPTOR (0.0): class HID
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 0
    bAlternateSetting: 0
    bNumEndpoints: 1
    bInterfaceClass: HID (0x03)
    bInterfaceSubClass: No Subclass (0x00)
    bInterfaceProtocol: 0x00
    iInterface: 0
UNKNOWN DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x21 (unknown)
ENDPOINT DESCRIPTOR
    bLength: 7
    bDescriptorType: 0x05 (ENDPOINT)
    bEndpointAddress: 0x81  IN  Endpoint:1
    bmAttributes: 0x03
    wMaxPacketSize: 32
    bInterval: 32

Frame 9: 36 bytes on wire (288 bits), 36 bytes captured (288 bits) on interface \\.\USBPcap2, id 0
USB URB
Setup Data
    bmRequestType: 0x21
    bRequest: 10
    wValue: 0x0000
    wIndex: 0 (0x0000)
    wLength: 0

Frame 11: 36 bytes on wire (288 bits), 36 bytes captured (288 bits) on interface \\.\USBPcap2, id 0
USB URB
Setup Data
    bmRequestType: 0x81
    bRequest: 6
    wValue: 0x2200
    wIndex: 0 (0x0000)
    wLength: 100

Frame 12: 64 bytes on wire (512 bits), 64 bytes captured (512 bits) on interface \\.\USBPcap2, id 0
USB URB
CONTROL response data: 0600ff0901a10119012902150025017501960001810219012902150025019600029102c0

0x06, 0x00, 0xFF,  // Usage Page (Vendor Defined 0xFF00)
0x09, 0x01,        // Usage (0x01)
0xA1, 0x01,        // Collection (Application)
0x19, 0x01,        //   Usage Minimum (0x01)
0x29, 0x02,        //   Usage Maximum (0x02)
0x15, 0x00,        //   Logical Minimum (0)
0x25, 0x01,        //   Logical Maximum (1)
0x75, 0x01,        //   Report Size (1)
0x96, 0x00, 0x01,  //   Report Count (256)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x19, 0x01,        //   Usage Minimum (0x01)
0x29, 0x02,        //   Usage Maximum (0x02)
0x15, 0x00,        //   Logical Minimum (0)
0x25, 0x01,        //   Logical Maximum (1)
0x96, 0x00, 0x02,  //   Report Count (512)
0x91, 0x02,        //   Output (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0xC0,              // End Collection

// 36 bytes

// best guess: USB HID Report Descriptor
```

### UsbTreeView

```text
    =========================== USB Port5 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 4-5
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path              : \\?\usb#vid_2f24&pid_0001#8&1265ce96&0&5#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_2F24&PID_0001\8&1265CE96&0&5
Hardware IDs             : USB\VID_2F24&PID_0001&REV_0120 USB\VID_2F24&PID_0001
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0085 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.19041.868  Date: 2021-04-18)
Driver Inf               : C:\WINDOWS\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0005.Hub_#0002
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(5), ACPI(_SB_)#ACPI(PCI0)#ACPI(BXBR)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT5)
Container ID             : {7180b222-4188-11ed-9452-fd82f29fe66d}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
EnhancedPowerMgmtEnabled : 1
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : HID-compliant vendor-defined device
  DevicePath             : \\?\hid#vid_2f24&pid_0001#9&119e0d87&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030}
  KernelName             : \Device\000001c3
  Device ID              : HID\VID_2F24&PID_0001\9&119E0D87&0&0000
  Class                  : HIDClass

        ---------------- Connection Information ---------------
Connection Index         : 0x05 (5)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x07 (7)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x01 (1 pipe to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 05 00 00 00 12 01 10 01 00 00 00 40 24 2F 01 00   ...........@$/..
                           20 01 01 02 00 01 01 01 00 07 00 01 00 00 00 01    ...............
                           00 00 00 07 05 81 03 20 00 20 00 00 00 00         ....... . ....

        --------------- Connection Information V2 -------------
Connection Index         : 0x05 (5)
Length                   : 0x10 (16 bytes)
SupportedUsbProtocols    : 0x03
 Usb110                  : 1 (yes)
 Usb200                  : 1 (yes)
 Usb300                  : 0 (no)
 ReservedMBZ             : 0x00
Flags                    : 0x00
 DevIsOpAtSsOrHigher     : 0 (Is not operating at SuperSpeed or higher)
 DevIsSsCapOrHigher      : 0 (Is not SuperSpeed capable or higher)
 DevIsOpAtSsPlusOrHigher : 0 (Is not operating at SuperSpeedPlus or higher)
 DevIsSsPlusCapOrHigher  : 0 (Is not SuperSpeedPlus capable or higher)
 ReservedMBZ             : 0x00
Data (HexDump)           : 05 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x110 (USB Version 1.10)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x2F24
idProduct                : 0x0001
bcdDevice                : 0x0120
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : " "
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Updater"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 10 01 00 00 00 40 24 2F 01 00 20 01 01 02   .......@$/.. ...
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0022 (34 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0x80
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0x32 (100 mA)
Data (HexDump)           : 09 02 22 00 01 01 00 80 32 09 04 00 00 01 03 00   ..".....2.......
                           00 00 09 21 11 01 00 01 22 24 00 07 05 81 03 20   ...!...."$..... 
                           00 20                                             . 

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
bAlternateSetting        : 0x00
bNumEndpoints            : 0x01 (1 Endpoint)
bInterfaceClass          : 0x03 (HID - Human Interface Device)
bInterfaceSubClass       : 0x00 (None)
bInterfaceProtocol       : 0x00 (None)
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 00 01 03 00 00 00                        .........

        ------------------- HID Descriptor --------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x21 (HID Descriptor)
bcdHID                   : 0x0111 (HID Version 1.11)
bCountryCode             : 0x00 (00 = not localized)
bNumDescriptors          : 0x01
Data (HexDump)           : 09 21 11 01 00 01 22 24 00                        .!...."$.
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0024 (36 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0020 (32 bytes)
bInterval                : 0x20 (32 ms)
Data (HexDump)           : 07 05 81 03 20 00 20                              .... . 

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : " "  *!*CAUTION  contains space characters only
Data (HexDump)           : 04 03 20 00                                       .. .
             ------ String Descriptor 2 ------
bLength                  : 0x10 (16 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Updater"
Data (HexDump)           : 10 03 55 00 70 00 64 00 61 00 74 00 65 00 72 00   ..U.p.d.a.t.e.r.
```

## NACON PS4 Compact Controller BB4469CGry

Connection sequence slightly differs between on PS and on Windows. The PS's first GET_DESCRIPTOR request has an 8 byte length while Windows uses 18 bytes. Another difference observed is that the PS firmware issues a SET_ADDRESS before the first GET_DESCRIPTOR whine on Windows this is the other way around. For now these are assumptions as proofing this is difficult without a custom USB stack.

![PpYyGBB2bl.png](images/PpYyGBB2bl.png)

### Wireshark decoding on PS mode

#### Configuration Descriptor

```text
Frame 457: 42 bytes on wire (336 bits), 42 bytes captured (336 bits)
USB Packet
USB URB
CONFIGURATION DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x02 (CONFIGURATION)
    wTotalLength: 231
    bNumInterfaces: 4
    bConfigurationValue: 1
    iConfiguration: 0
    Configuration bmAttributes: 0x80  NOT SELF-POWERED  NO REMOTE-WAKEUP
        1... .... = Must be 1: Must be 1 for USB 1.1 and higher
        .0.. .... = Self-Powered: This device is powered from the USB bus
        ..0. .... = Remote Wakeup: This device does NOT support remote wakeup
    bMaxPower: 250  (500mA)
INTERFACE DESCRIPTOR (0.0): class Audio
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 0
    bAlternateSetting: 0
    bNumEndpoints: 0
    bInterfaceClass: Audio (0x01)
    bInterfaceSubClass: Audio Control (0x01)
    bInterfaceProtocol: 0x00
    iInterface: 0
Class-specific Audio Control Interface Descriptor: Header Descriptor
    bLength: 10
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Header Descriptor (0x01)
    Version: 1.00
    Total length: 71
    Total number of interfaces: 2
    Interface number: 1
    Interface number: 2
Class-specific Audio Control Interface Descriptor: Input terminal descriptor
    bLength: 12
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Input terminal descriptor (0x02)
    Terminal ID: 1
    Terminal Type: USB Streaming (0x0101)
    Assoc Terminal: 6
    Number Channels: 2
    Channel Config: 0x0003, Left Front, Right Front
        .... .... .... ...1 = Left Front: True
        .... .... .... ..1. = Right Front: True
        .... .... .... .0.. = Center Front: False
        .... .... .... 0... = Low Frequency Enhancement: False
        .... .... ...0 .... = Left Surround: False
        .... .... ..0. .... = Right Surround: False
        .... .... .0.. .... = Left of Center: False
        .... .... 0... .... = Right of Center: False
        .... ...0 .... .... = Surround: False
        .... ..0. .... .... = Side Left: False
        .... .0.. .... .... = Side Right: False
        .... 0... .... .... = Top: False
        0000 .... .... .... = Reserved: 0x0
    Channel Names: 0
    String descriptor index: 0
Class-specific Audio Control Interface Descriptor: Feature unit descriptor
    bLength: 10
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Feature unit descriptor (0x06)
    Unit ID: 2
    Source ID: 1
    Control Size: 1
    Controls: 030000
        Master channel 0 Control: 0x03, Mute, Volume
            .... ...1 = Mute: True
            .... ..1. = Volume: True
            .... .0.. = Bass: False
            .... 0... = Mid: False
            ...0 .... = Treble: False
            ..0. .... = Graphic Equalizer: False
            .0.. .... = Automatic Gain: False
            0... .... = Delay: False
        Logical channel 1 Control: 0x00
            .... ...0 = Mute: False
            .... ..0. = Volume: False
            .... .0.. = Bass: False
            .... 0... = Mid: False
            ...0 .... = Treble: False
            ..0. .... = Graphic Equalizer: False
            .0.. .... = Automatic Gain: False
            0... .... = Delay: False
        Logical channel 2 Control: 0x00
            .... ...0 = Mute: False
            .... ..0. = Volume: False
            .... .0.. = Bass: False
            .... 0... = Mid: False
            ...0 .... = Treble: False
            ..0. .... = Graphic Equalizer: False
            .0.. .... = Automatic Gain: False
            0... .... = Delay: False
    Feature: 0
Class-specific Audio Control Interface Descriptor: Output terminal descriptor
    bLength: 9
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Output terminal descriptor (0x03)
    Terminal ID: 3
    Terminal Type: Headset (0x0402)
    Assoc Terminal: 4
    Source ID: 2
    String descriptor index: 0
Class-specific Audio Control Interface Descriptor: Input terminal descriptor
    bLength: 12
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Input terminal descriptor (0x02)
    Terminal ID: 4
    Terminal Type: Headset (0x0402)
    Assoc Terminal: 3
    Number Channels: 1
    Channel Config: 0x0000
        .... .... .... ...0 = Left Front: False
        .... .... .... ..0. = Right Front: False
        .... .... .... .0.. = Center Front: False
        .... .... .... 0... = Low Frequency Enhancement: False
        .... .... ...0 .... = Left Surround: False
        .... .... ..0. .... = Right Surround: False
        .... .... .0.. .... = Left of Center: False
        .... .... 0... .... = Right of Center: False
        .... ...0 .... .... = Surround: False
        .... ..0. .... .... = Side Left: False
        .... .0.. .... .... = Side Right: False
        .... 0... .... .... = Top: False
        0000 .... .... .... = Reserved: 0x0
    Channel Names: 0
    String descriptor index: 0
Class-specific Audio Control Interface Descriptor: Feature unit descriptor
    bLength: 9
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Feature unit descriptor (0x06)
    Unit ID: 5
    Source ID: 4
    Control Size: 1
    Controls: 0300
        Master channel 0 Control: 0x03, Mute, Volume
            .... ...1 = Mute: True
            .... ..1. = Volume: True
            .... .0.. = Bass: False
            .... 0... = Mid: False
            ...0 .... = Treble: False
            ..0. .... = Graphic Equalizer: False
            .0.. .... = Automatic Gain: False
            0... .... = Delay: False
        Logical channel 1 Control: 0x00
            .... ...0 = Mute: False
            .... ..0. = Volume: False
            .... .0.. = Bass: False
            .... 0... = Mid: False
            ...0 .... = Treble: False
            ..0. .... = Graphic Equalizer: False
            .0.. .... = Automatic Gain: False
            0... .... = Delay: False
    Feature: 0
Class-specific Audio Control Interface Descriptor: Output terminal descriptor
    bLength: 9
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Output terminal descriptor (0x03)
    Terminal ID: 6
    Terminal Type: USB Streaming (0x0101)
    Assoc Terminal: 1
    Source ID: 5
    String descriptor index: 0
INTERFACE DESCRIPTOR (1.0): class Audio
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 1
    bAlternateSetting: 0
    bNumEndpoints: 0
    bInterfaceClass: Audio (0x01)
    bInterfaceSubClass: Audio Streaming (0x02)
    bInterfaceProtocol: 0x00
    iInterface: 0
INTERFACE DESCRIPTOR (1.1): class Audio
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 1
    bAlternateSetting: 1
    bNumEndpoints: 1
    bInterfaceClass: Audio (0x01)
    bInterfaceSubClass: Audio Streaming (0x02)
    bInterfaceProtocol: 0x00
    iInterface: 0
Class-specific Audio Streaming Interface Descriptor: General AS Descriptor
    bLength: 7
    bDescriptorType: 0x24 (audio class interface)
    Subtype: General AS Descriptor (0x01)
    Connected Terminal ID: 1
    Interface delay in frames: 1
    Format: PCM (0x0001)
Class-specific Audio Streaming Interface Descriptor: Format type descriptor
    bLength: 14
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Format type descriptor (0x02)
    FormatType: 1
    Number Channels: 2
    Subframe Size: 2
    Bit Resolution: 16
    Samples Frequence Type: 2
    Samples Frequence: 32000
    Samples Frequence: 48000
ENDPOINT DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x05 (ENDPOINT)
    bEndpointAddress: 0x01  OUT  Endpoint:1
        0... .... = Direction: OUT Endpoint
        .... 0001 = Endpoint Number: 0x1
    bmAttributes: 0x09
        .... ..01 = Transfertype: Isochronous-Transfer (0x1)
        .... 10.. = Synchronisationtype: Adaptive (0x2)
        ..00 .... = Behaviourtype: Data-Endpoint (0x0)
    wMaxPacketSize: 196
        ...0 0... .... .... = Transactions per microframe: 1 (0)
        .... ..00 1100 0100 = Maximum Packet Size: 196
    bInterval: 1
    bRefresh: 0
    bSynchAddress: 0
Class-specific Audio Streaming Endpoint Descriptor
    bLength: 7
    bDescriptorType: 0x25 (audio class endpoint)
    Subtype: General Descriptor (0x01)
    Attributes: 0x01, Sampling Frequency Control
        .... ...1 = Sampling Frequency Control: True
        .... ..0. = Pitch Control: False
        .000 00.. = Reserved: 0x00
        0... .... = MaxPacketsOnly: False
    Lock Delay Units: Undefined (0)
    Lock Delay: 0
INTERFACE DESCRIPTOR (2.0): class Audio
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 2
    bAlternateSetting: 0
    bNumEndpoints: 0
    bInterfaceClass: Audio (0x01)
    bInterfaceSubClass: Audio Streaming (0x02)
    bInterfaceProtocol: 0x00
    iInterface: 0
INTERFACE DESCRIPTOR (2.1): class Audio
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 2
    bAlternateSetting: 1
    bNumEndpoints: 1
    bInterfaceClass: Audio (0x01)
    bInterfaceSubClass: Audio Streaming (0x02)
    bInterfaceProtocol: 0x00
    iInterface: 0
Class-specific Audio Streaming Interface Descriptor: General AS Descriptor
    bLength: 7
    bDescriptorType: 0x24 (audio class interface)
    Subtype: General AS Descriptor (0x01)
    Connected Terminal ID: 6
    Interface delay in frames: 1
    Format: PCM (0x0001)
Class-specific Audio Streaming Interface Descriptor: Format type descriptor
    bLength: 14
    bDescriptorType: 0x24 (audio class interface)
    Subtype: Format type descriptor (0x02)
    FormatType: 1
    Number Channels: 1
    Subframe Size: 2
    Bit Resolution: 16
    Samples Frequence Type: 2
    Samples Frequence: 16000
    Samples Frequence: 48000
ENDPOINT DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x05 (ENDPOINT)
    bEndpointAddress: 0x82  IN  Endpoint:2
        1... .... = Direction: IN Endpoint
        .... 0010 = Endpoint Number: 0x2
    bmAttributes: 0x05
        .... ..01 = Transfertype: Isochronous-Transfer (0x1)
        .... 01.. = Synchronisationtype: Asynchronous (0x1)
        ..00 .... = Behaviourtype: Data-Endpoint (0x0)
    wMaxPacketSize: 98
        ...0 0... .... .... = Transactions per microframe: 1 (0)
        .... ..00 0110 0010 = Maximum Packet Size: 98
    bInterval: 1
    bRefresh: 0
    bSynchAddress: 0
Class-specific Audio Streaming Endpoint Descriptor
    bLength: 7
    bDescriptorType: 0x25 (audio class endpoint)
    Subtype: General Descriptor (0x01)
    Attributes: 0x01, Sampling Frequency Control
        .... ...1 = Sampling Frequency Control: True
        .... ..0. = Pitch Control: False
        .000 00.. = Reserved: 0x00
        0... .... = MaxPacketsOnly: False
    Lock Delay Units: Undefined (0)
    Lock Delay: 0
INTERFACE DESCRIPTOR (3.0): class HID
    bLength: 9
    bDescriptorType: 0x04 (INTERFACE)
    bInterfaceNumber: 3
    bAlternateSetting: 0
    bNumEndpoints: 2
    bInterfaceClass: HID (0x03)
    bInterfaceSubClass: No Subclass (0x00)
    bInterfaceProtocol: 0x00
    iInterface: 0
UNKNOWN DESCRIPTOR
    bLength: 9
    bDescriptorType: 0x21 (unknown)
ENDPOINT DESCRIPTOR
    bLength: 7
    bDescriptorType: 0x05 (ENDPOINT)
    bEndpointAddress: 0x84  IN  Endpoint:4
        1... .... = Direction: IN Endpoint
        .... 0100 = Endpoint Number: 0x4
    bmAttributes: 0x03
        .... ..11 = Transfertype: Interrupt-Transfer (0x3)
    wMaxPacketSize: 64
        ...0 0... .... .... = Transactions per microframe: 1 (0)
        .... ..00 0100 0000 = Maximum Packet Size: 64
    bInterval: 5
ENDPOINT DESCRIPTOR
    bLength: 7
    bDescriptorType: 0x05 (ENDPOINT)
    bEndpointAddress: 0x03  OUT  Endpoint:3
        0... .... = Direction: OUT Endpoint
        .... 0011 = Endpoint Number: 0x3
    bmAttributes: 0x03
        .... ..11 = Transfertype: Interrupt-Transfer (0x3)
    wMaxPacketSize: 64
        ...0 0... .... .... = Transactions per microframe: 1 (0)
        .... ..00 0100 0000 = Maximum Packet Size: 64
    bInterval: 5

```

#### HID Report Descriptor

```text
0x05, 0x01,        // Usage Page (Generic Desktop Ctrls)
0x09, 0x05,        // Usage (Game Pad)
0xA1, 0x01,        // Collection (Application)
0x85, 0x01,        //   Report ID (1)
0x09, 0x30,        //   Usage (X)
0x09, 0x31,        //   Usage (Y)
0x09, 0x32,        //   Usage (Z)
0x09, 0x35,        //   Usage (Rz)
0x15, 0x00,        //   Logical Minimum (0)
0x26, 0xFF, 0x00,  //   Logical Maximum (255)
0x75, 0x08,        //   Report Size (8)
0x95, 0x04,        //   Report Count (4)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x39,        //   Usage (Hat switch)
0x15, 0x00,        //   Logical Minimum (0)
0x25, 0x07,        //   Logical Maximum (7)
0x35, 0x00,        //   Physical Minimum (0)
0x46, 0x3B, 0x01,  //   Physical Maximum (315)
0x65, 0x14,        //   Unit (System: English Rotation, Length: Centimeter)
0x75, 0x04,        //   Report Size (4)
0x95, 0x01,        //   Report Count (1)
0x81, 0x42,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State)
0x65, 0x00,        //   Unit (None)
0x05, 0x09,        //   Usage Page (Button)
0x19, 0x01,        //   Usage Minimum (0x01)
0x29, 0x0E,        //   Usage Maximum (0x0E)
0x15, 0x00,        //   Logical Minimum (0)
0x25, 0x01,        //   Logical Maximum (1)
0x75, 0x01,        //   Report Size (1)
0x95, 0x0E,        //   Report Count (14)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x06, 0x00, 0xFF,  // Usage Page (Vendor Defined 0xFF00)
0x09, 0x20,        // Usage (0x20)
0x75, 0x06,        // Report Size (6)
0x95, 0x01,        // Report Count (1)
0x81, 0x02,        // Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x01,        // Usage Page (Generic Desktop Ctrls)
0x09, 0x33,        // Usage (Rx)
0x09, 0x34,        // Usage (Ry)
0x15, 0x00,        // Logical Minimum (0)
0x26, 0xFF, 0x00,  // Logical Maximum (255)
0x75, 0x08,        // Report Size (8)
0x95, 0x02,        // Report Count (2)
0x81, 0x02,        // Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x06, 0x00, 0xFF,  // Usage Page (Vendor Defined 0xFF00)
0x09, 0x21,        // Usage (0x21)
0x95, 0x36,        // Report Count (54)
0x81, 0x02,        // Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x85, 0x05,        // Report ID (5)
0x09, 0x22,        // Usage (0x22)
0x95, 0x1F,        // Report Count (31)
0x91, 0x02,        // Output (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x85, 0x03,        // Report ID (3)
0x0A, 0x21, 0x27,  // Usage (0x2721)
0x95, 0x2F,        // Report Count (47)
0xB1, 0x02,        // Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x06, 0x80, 0xFF,  // Usage Page (Vendor Defined 0xFF80)
0x85, 0xE0,        // Report ID (-32)
0x09, 0x57,        // Usage (0x57)
0x95, 0x02,        // Report Count (2)
0xB1,              // Feature (Data,Array,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x02, 0xC0, 0x06,  // Unknown (bTag: 0x00, bType: 0x00)
0xF0,              // Unknown (bTag: 0x0F, bType: 0x00)
0xFF, 0x09, 0x40, 0xA1, 0x01,  // Unknown (bTag: 0x0F, bType: 0x03)
0x85, 0xF0,        // Report ID (-16)
0x09, 0x47,        // Usage (0x47)
0x95, 0x3F,        // Report Count (63)
0xB1, 0x02,        // Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x85, 0xF1,        // Report ID (-15)
0x09, 0x48,        // Usage (0x48)
0x95, 0x3F,        // Report Count (63)
0xB1, 0x02,        // Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x85, 0xF2,        // Report ID (-14)
0x09, 0x49,        // Usage (0x49)
0x95, 0x0F,        // Report Count (15)
0xB1, 0x02,        // Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x85, 0xF3,        // Report ID (-13)
0x0A, 0x01, 0x47,  // Usage (0x4701)
0x95, 0x07,        // Report Count (7)
0xB1, 0x02,        // Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0xC0,              // End Collection
```

### UsbTreeView (WinSUB)

```text

    =========================== USB Port10 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 2-10

      ========================== Summary =========================
Vendor ID                : 0x146B (BigBen Interactive Limited)
Product ID               : 0x0603
USB Version              : 2.0 -> but Device is Full-Speed only
Port maximum Speed       : High-Speed
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : no
Demanded Current         : 500 mA
Used Endpoints           : 3

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Friendly Name            : PC Compact Controller
Device Description       : WinUsb Device
Device Path 1            : \\?\USB#VID_CEA0&PID_D200#04E028E1#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Device Path 2            : \\?\USB#VID_CEA0&PID_D200#04E028E1#{86431f5b-9f5a-48ce-8fbf-a537413ef358}
Kernel Name              : \Device\USBPDO-10
Device ID                : USB\VID_CEA0&PID_D200\04E028E1
Hardware IDs             : USB\VID_CEA0&PID_D200
Driver KeyName           : {88bae032-5a81-49f0-bc3d-a4ff138216d6}\0001 (GUID_DEVCLASS_USBDEVICE)
Driver                   : \SystemRoot\System32\drivers\WinUSB.sys (Version: 10.0.19041.1  Date: 2019-12-07)
Driver Inf               : C:\WINDOWS\inf\winusb.inf
Legacy BusType           : PNPBus
Class                    : USBDevice
Class GUID               : {88bae032-5a81-49f0-bc3d-a4ff138216d6} (GUID_DEVCLASS_USBDEVICE)
Service                  : WINUSB
Enumerator               : USB
Location Info            : Port_#0010.Hub_#0001
Location IDs             : PCIROOT(0)#PCI(1400)#USBROOT(0)#USB(10), ACPI(_SB_)#ACPI(PCI0)#ACPI(XHC_)#ACPI(RHUB)#ACPI(HS10)
Container ID             : {a581e49f-cc24-507b-9b10-f90fbae6d1e2}
Manufacturer Info        : WinUsb Device
Capabilities             : 0x14 (Removable, UniqueID)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
HcDisableSelectiveSuspend: 0
EnableSelectiveSuspend   : 0
SelectiveSuspendEnabled  : 0
EnhancedPowerMgmtEnabled : 0
IdleInWorkingState       : 0
WakeFromSleepState       : 0
Power State              : D0 (supported: D0, D3, wake from D0)

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\146B06030100
 osvc                    : REG_BINARY 01 90
 SkipContainerIdQuery    : REG_BINARY 01 00

        ---------------- Connection Information ---------------
Connection Index         : 0x0A (Port 10)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x0E (14)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=64    bInterval=4
Pipe[1]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=64    bInterval=8
Data (HexDump)           : 0A 00 00 00 12 01 00 02 FF FF FF 40 6B 14 03 06   ...........@k...
                           00 01 01 02 03 01 01 01 00 0E 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 40 00 04 00 00 00 00 07 05   .......@........
                           02 03 40 00 08 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x0A (10)
Length                   : 0x10 (16 bytes)
SupportedUsbProtocols    : 0x03
 Usb110                  : 1 (yes, port supports USB 1.1)
 Usb200                  : 1 (yes, port supports USB 2.0)
 Usb300                  : 0 (no, port not supports USB 3.0)
 ReservedMBZ             : 0x00
Flags                    : 0x00
 DevIsOpAtSsOrHigher     : 0 (Device is not operating at SuperSpeed or higher)
 DevIsSsCapOrHigher      : 0 (Device is not SuperSpeed capable or higher)
 DevIsOpAtSsPlusOrHigher : 0 (Device is not operating at SuperSpeedPlus or higher)
 DevIsSsPlusCapOrHigher  : 0 (Device is not SuperSpeedPlus capable or higher)
 ReservedMBZ             : 0x00
Data (HexDump)           : 0A 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.0) -> but device is Full-Speed only
bDeviceClass             : 0xFF (Vendor Specific)
bDeviceSubClass          : 0xFF
bDeviceProtocol          : 0xFF
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x146B (BigBen Interactive Limited)
idProduct                : 0x0603
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Bigben Interactive"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "PC Compact Controller"
iSerialNumber            : 0x03 (String Descriptor 3)
 Language 0x0409         : "04E028E1"
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 FF FF FF 40 6B 14 03 06 00 01 01 02   .......@k.......
                           03 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0031 (49 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0x80
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 02 31 00 01 01 00 80 FA 09 04 00 00 02 FF 5D   ..1............]
                           01 00 11 21 00 01 01 25 81 14 00 00 00 00 13 02   ...!...%........
                           08 03 03 07 05 81 03 40 00 04 07 05 02 03 40 00   .......@......@.
                           08                                                .

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00 (Interface 0)
bAlternateSetting        : 0x00
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x5D
bInterfaceProtocol       : 0x01
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 00 02 FF 5D 01 00                        ......]..

        ----------------- Unknown Descriptor ------------------
bLength                  : 0x11 (17 bytes)
bDescriptorType          : 0x21
Data (HexDump)           : 11 21 00 01 01 25 81 14 00 00 00 00 13 02 08 03 
                           03 

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 81 03 40 00 04                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x08 (8 ms)
Data (HexDump)           : 07 05 02 03 40 00 08                              ....@..

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE  (because the device is Full-Speed only)

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x26 (38 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Bigben Interactive"
Data (HexDump)           : 26 03 42 00 69 00 67 00 62 00 65 00 6E 00 20 00   &.B.i.g.b.e.n. .
                           49 00 6E 00 74 00 65 00 72 00 61 00 63 00 74 00   I.n.t.e.r.a.c.t.
                           69 00 76 00 65 00                                 i.v.e.
             ------ String Descriptor 2 ------
bLength                  : 0x2C (44 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "PC Compact Controller"
Data (HexDump)           : 2C 03 50 00 43 00 20 00 43 00 6F 00 6D 00 70 00   ,.P.C. .C.o.m.p.
                           61 00 63 00 74 00 20 00 43 00 6F 00 6E 00 74 00   a.c.t. .C.o.n.t.
                           72 00 6F 00 6C 00 6C 00 65 00 72 00               r.o.l.l.e.r.
             ------ String Descriptor 3 ------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "04E028E1"
Data (HexDump)           : 12 03 30 00 34 00 45 00 30 00 32 00 38 00 45 00   ..0.4.E.0.2.8.E.
                           31 00                                             1.
```

### lsusb

```text
lsusb -vd 146b:0603

Bus 001 Device 004: ID 146b:0603 BigBen Interactive PC Compact Controller
Couldn't open device, some information will be missing
Device Descriptor:
  bLength                18
  bDescriptorType         1
  bcdUSB               2.00
  bDeviceClass          255 Vendor Specific Class
  bDeviceSubClass       255 Vendor Specific Subclass
  bDeviceProtocol       255 Vendor Specific Protocol
  bMaxPacketSize0        64
  idVendor           0x146b BigBen Interactive
  idProduct          0x0603
  bcdDevice            1.00
  iManufacturer           1 Bigben Interactive
  iProduct                2 PC Compact Controller
  iSerial                 3 04E028E1
  bNumConfigurations      1
  Configuration Descriptor:
    bLength                 9
    bDescriptorType         2
    wTotalLength       0x0031
    bNumInterfaces          1
    bConfigurationValue     1
    iConfiguration          0
    bmAttributes         0x80
      (Bus Powered)
    MaxPower              500mA
    Interface Descriptor:
      bLength                 9
      bDescriptorType         4
      bInterfaceNumber        0
      bAlternateSetting       0
      bNumEndpoints           2
      bInterfaceClass       255 Vendor Specific Class
      bInterfaceSubClass     93
      bInterfaceProtocol      1
      iInterface              0
      ** UNRECOGNIZED:  11 21 00 01 01 25 81 14 00 00 00 00 13 02 08 03 03
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x81  EP 1 IN
        bmAttributes            3
          Transfer Type            Interrupt
          Synch Type               None
          Usage Type               Data
        wMaxPacketSize     0x0040  1x 64 bytes
        bInterval               4
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x02  EP 2 OUT
        bmAttributes            3
          Transfer Type            Interrupt
          Synch Type               None
          Usage Type               Data
        wMaxPacketSize     0x0040  1x 64 bytes
        bInterval               8
```
