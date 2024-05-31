# Retro Fighters Defender Bluetooth Edition

## Linux

### `lsusb`

```bash
lsusb -s 003:004 -vvv

Bus 003 Device 004: ID 054c:05c4 Sony Corp. DualShock 4 [CUH-ZCT1x]
Device Descriptor:
  bLength                18
  bDescriptorType         1
  bcdUSB               2.00
  bDeviceClass            0 
  bDeviceSubClass         0 
  bDeviceProtocol         0 
  bMaxPacketSize0        64
  idVendor           0x054c Sony Corp.
  idProduct          0x05c4 DualShock 4 [CUH-ZCT1x]
  bcdDevice            2.21
  iManufacturer           1 Sony Computer Entertainment
  iProduct                2 Wireless Controller
  iSerial                 0 
  bNumConfigurations      1
  Configuration Descriptor:
    bLength                 9
    bDescriptorType         2
    wTotalLength       0x0029
    bNumInterfaces          1
    bConfigurationValue     1
    iConfiguration          0 
    bmAttributes         0xc0
      Self Powered
    MaxPower              500mA
    Interface Descriptor:
      bLength                 9
      bDescriptorType         4
      bInterfaceNumber        0
      bAlternateSetting       0
      bNumEndpoints           2
      bInterfaceClass         3 Human Interface Device
      bInterfaceSubClass      0 
      bInterfaceProtocol      0 
      iInterface              0 
        HID Device Descriptor:
          bLength                 9
          bDescriptorType        33
          bcdHID               1.11
          bCountryCode            0 Not supported
          bNumDescriptors         1
          bDescriptorType        34 Report
          wDescriptorLength     467
         Report Descriptors: 
           ** UNAVAILABLE **
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x81  EP 1 IN
        bmAttributes            3
          Transfer Type            Interrupt
          Synch Type               None
          Usage Type               Data
        wMaxPacketSize     0x0040  1x 64 bytes
        bInterval               5
      Endpoint Descriptor:
        bLength                 7
        bDescriptorType         5
        bEndpointAddress     0x02  EP 2 OUT
        bmAttributes            3
          Transfer Type            Interrupt
          Synch Type               None
          Usage Type               Data
        wMaxPacketSize     0x0040  1x 64 bytes
        bInterval               5
can't get device qualifier: Resource temporarily unavailable
can't get debug descriptor: Resource temporarily unavailable
Device Status:     0x0000
  (Bus Powered)
``` 

## XInput Mode (Default)

### USBTreeViewer

```text

    =========================== USB Port7 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 1-7
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no
ConnectionIndex          : 0x07 (Port 7)
CompanionIndex           : 0
 CompanionHubSymLnk      : USB#ROOT_HUB30#5&32dfb9bc&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
 CompanionPortNumber     : 0x03 (Port 3)
 -> CompanionPortChain   : 1-3

      ========================== Summary =========================
Vendor ID                : 0x045E (Microsoft Corporation)
Product ID               : 0x028E
USB Version              : 1.1
Port maximum Speed       : High-Speed (Companion Port 1-3 is doing the SuperSpeed)
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : no
Demanded Current         : 500 mA
Used Endpoints           : 3

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : Xbox 360 Controller for Windows
Device Path 1            : \\?\USB#VID_045E&PID_028E#Shanwan202107142050#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Device Path 2            : \\?\USB#VID_045E&PID_028E#Shanwan202107142050#{ec87f1e3-c13b-4100-b5f7-8b84d54260cb}
Kernel Name              : \Device\USBPDO-10
Device ID                : USB\VID_045E&PID_028E\SHANWAN202107142050
Hardware IDs             : USB\VID_045E&PID_028E&REV_0110 USB\VID_045E&PID_028E
Driver KeyName           : {d61ca365-5af4-4486-998b-9db4734c6ca3}\0000
Driver                   : \SystemRoot\System32\drivers\xusb22.sys (Version: 10.0.22621.3374  Date: 2024-03-26  Company: Microsoft Corporation)
Driver Inf               : C:\Windows\inf\xusb22.inf
Legacy BusType           : PNPBus
Class                    : XnaComposite
Class GUID               : {d61ca365-5af4-4486-998b-9db4734c6ca3}
Service                  : xusb22
Enumerator               : USB
Location Info            : Port_#0007.Hub_#0001
Address                  : 7
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#USBROOT(0)#USB(7), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP1)#ACPI(PTXH)#ACPI(RHUB)#ACPI(PO7_)
Container ID             : {2ff19da7-374d-5b65-8581-eb1acb95ac7e}
Manufacturer Info        : Microsoft
Capabilities             : 0x94 (Removable, UniqueID, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Power State              : D0 (supported: D0, D3, wake from D0)

        ---------------- Connection Information ---------------
Connection Index         : 0x07 (Port 7)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x1D (29)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number of open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x20    bInterval=8   -> 420 Bits/ms = 52500 Bytes/s
Pipe[1]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x20    bInterval=8   -> 420 Bits/ms = 52500 Bytes/s
Data (HexDump)           : 07 00 00 00 12 01 10 01 FF FF FF 40 5E 04 8E 02   ...........@^...
                           10 01 01 02 03 01 01 01 00 1D 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 20 00 08 00 00 00 00 07 05   ....... ........
                           02 03 20 00 08 00 00 00 00                        .. ......

        --------------- Connection Information V2 -------------
Connection Index         : 0x07 (7)
Length                   : 0x10 (16 bytes)
SupportedUsbProtocols    : 0x03
 Usb110                  : 1 (yes, port supports USB 1.1)
 Usb200                  : 1 (yes, port supports USB 2.0)
 Usb300                  : 0 (no, port not supports USB 3.0) -> but Companion Port 1-3 does
 ReservedMBZ             : 0x00
Flags                    : 0x00
 DevIsOpAtSsOrHigher     : 0 (Device is not operating at SuperSpeed or higher)
 DevIsSsCapOrHigher      : 0 (Device is not SuperSpeed capable or higher)
 DevIsOpAtSsPlusOrHigher : 0 (Device is not operating at SuperSpeedPlus or higher)
 DevIsSsPlusCapOrHigher  : 0 (Device is not SuperSpeedPlus capable or higher)
 ReservedMBZ             : 0x00
Data (HexDump)           : 07 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x110 (USB Version 1.1)
bDeviceClass             : 0xFF (Vendor Specific)
bDeviceSubClass          : 0xFF
bDeviceProtocol          : 0xFF
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x045E (Microsoft Corporation)
idProduct                : 0x028E
bcdDevice                : 0x0110
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "shanwan"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Xbox360 For Windows"
iSerialNumber            : 0x03 (String Descriptor 3)
 Language 0x0409         : "Shanwan202107142050"
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 10 01 FF FF FF 40 5E 04 8E 02 10 01 01 02   .......@^.......
                           03 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0030 (48 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0x80
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)

Data (HexDump)           : 09 02 30 00 01 01 00 80 FA 09 04 00 00 02 FF 5D   ..0............]
                           01 00 10 21 10 01 01 24 81 14 03 00 03 13 02 00   ...!...$........
                           03 00 07 05 81 03 20 00 08 07 05 02 03 20 00 08   ...... ...... ..

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
bLength                  : 0x10 (16 bytes)
bDescriptorType          : 0x21
Data (HexDump)           : 10 21 10 01 01 24 81 14 03 00 03 13 02 00 03 00 
                           
        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0020 (32 bytes)
bInterval                : 0x08 (8 ms)
Data (HexDump)           : 07 05 81 03 20 00 08                              .... ..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0020 (32 bytes)
bInterval                : 0x08 (8 ms)
Data (HexDump)           : 07 05 02 03 20 00 08                              .... ..

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x10 (16 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "shanwan"
Data (HexDump)           : 10 03 73 00 68 00 61 00 6E 00 77 00 61 00 6E 00   ..s.h.a.n.w.a.n.
             ------ String Descriptor 2 ------
bLength                  : 0x28 (40 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Xbox360 For Windows"
Data (HexDump)           : 28 03 58 00 62 00 6F 00 78 00 33 00 36 00 30 00   (.X.b.o.x.3.6.0.
                           20 00 46 00 6F 00 72 00 20 00 57 00 69 00 6E 00    .F.o.r. .W.i.n.
                           64 00 6F 00 77 00 73 00                           d.o.w.s.
             ------ String Descriptor 3 ------
bLength                  : 0x28 (40 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Shanwan202107142050"
Data (HexDump)           : 28 03 53 00 68 00 61 00 6E 00 77 00 61 00 6E 00   (.S.h.a.n.w.a.n.
                           32 00 30 00 32 00 31 00 30 00 37 00 31 00 34 00   2.0.2.1.0.7.1.4.
                           32 00 30 00 35 00 30 00                           2.0.5.0.
```

## DirectInput Mode

### USBTreeViewer

```text

    =========================== USB Port7 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 1-7
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no
ConnectionIndex          : 0x07 (Port 7)
CompanionIndex           : 0
 CompanionHubSymLnk      : USB#ROOT_HUB30#5&32dfb9bc&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
 CompanionPortNumber     : 0x03 (Port 3)
 -> CompanionPortChain   : 1-3

      ========================== Summary =========================
Vendor ID                : 0x2563 (Shenzhen ShanWan Technology Co., Ltd.)
Product ID               : 0x0575
USB Version              : 1.1
Port maximum Speed       : High-Speed (Companion Port 1-3 is doing the SuperSpeed)
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : no
Demanded Current         : 500 mA
Used Endpoints           : 3

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path              : \\?\USB#VID_2563&PID_0575#6&2f985c08&0&7#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Kernel Name              : \Device\USBPDO-11
Device ID                : USB\VID_2563&PID_0575\6&2F985C08&0&7
Hardware IDs             : USB\VID_2563&PID_0575&REV_0100 USB\VID_2563&PID_0575
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0033 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.22621.3527  Date: 2024-04-26  Company: Microsoft Corporation)
Driver Inf               : C:\Windows\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0007.Hub_#0001
Address                  : 7
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#USBROOT(0)#USB(7), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP1)#ACPI(PTXH)#ACPI(RHUB)#ACPI(PO7_)
Container ID             : {1f839908-0432-11ef-8806-d843ae1a79f7}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
SelectiveSuspendEnabled  : 0
EnhancedPowerMgmtEnabled : 1
Power State              : D0 (supported: D0, D3, wake from D0)

        ---------------- Connection Information ---------------
Connection Index         : 0x07 (Port 7)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x1E (30)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number of open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x40    bInterval=8   -> 718 Bits/ms = 89750 Bytes/s
Pipe[1]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x40    bInterval=8   -> 718 Bits/ms = 89750 Bytes/s
Data (HexDump)           : 07 00 00 00 12 01 10 01 00 00 00 40 63 25 75 05   ...........@c%u.
                           00 01 01 02 00 01 01 01 00 1E 00 02 00 00 00 01   ................
                           00 00 00 07 05 02 03 40 00 08 00 00 00 00 07 05   .......@........
                           81 03 40 00 08 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x07 (7)
Length                   : 0x10 (16 bytes)
SupportedUsbProtocols    : 0x03
 Usb110                  : 1 (yes, port supports USB 1.1)
 Usb200                  : 1 (yes, port supports USB 2.0)
 Usb300                  : 0 (no, port not supports USB 3.0) -> but Companion Port 1-3 does
 ReservedMBZ             : 0x00
Flags                    : 0x00
 DevIsOpAtSsOrHigher     : 0 (Device is not operating at SuperSpeed or higher)
 DevIsSsCapOrHigher      : 0 (Device is not SuperSpeed capable or higher)
 DevIsOpAtSsPlusOrHigher : 0 (Device is not operating at SuperSpeedPlus or higher)
 DevIsSsPlusCapOrHigher  : 0 (Device is not SuperSpeedPlus capable or higher)
 ReservedMBZ             : 0x00
Data (HexDump)           : 07 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x110 (USB Version 1.1)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x2563 (Shenzhen ShanWan Technology Co., Ltd.)
idProduct                : 0x0575
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "shanwan"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "X-D GamePad"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 10 01 00 00 00 40 63 25 75 05 00 01 01 02   .......@c%u.....
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0029 (41 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0x80
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)

Data (HexDump)           : 09 02 29 00 01 01 00 80 FA 09 04 00 00 02 03 00   ..).............
                           00 00 09 21 11 01 00 01 22 89 00 07 05 02 03 40   ...!...."......@
                           00 08 07 05 81 03 40 00 08                        ......@..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00 (Interface 0)
bAlternateSetting        : 0x00
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0x03 (HID - Human Interface Device)
bInterfaceSubClass       : 0x00 (None)
bInterfaceProtocol       : 0x00 (None)
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 00 02 03 00 00 00                        .........

        ------------------- HID Descriptor --------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x21 (HID Descriptor)
bcdHID                   : 0x0111 (HID Version 1.11)
bCountryCode             : 0x00 (00 = not localized)
bNumDescriptors          : 0x01
Data (HexDump)           : 09 21 11 01 00 01 22 89 00                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0089 (137 bytes)
Error reading descriptor : ERROR_GEN_FAILURE (due to a obscure limitation of the Win32 USB API, see F1 Help)

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x08 (8 ms)
Data (HexDump)           : 07 05 02 03 40 00 08                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x08 (8 ms)
Data (HexDump)           : 07 05 81 03 40 00 08                              ....@..

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x10 (16 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "shanwan"
Data (HexDump)           : 10 03 73 00 68 00 61 00 6E 00 77 00 61 00 6E 00   ..s.h.a.n.w.a.n.
             ------ String Descriptor 2 ------
bLength                  : 0x18 (24 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "X-D GamePad"
Data (HexDump)           : 18 03 58 00 2D 00 44 00 20 00 47 00 61 00 6D 00   ..X.-.D. .G.a.m.
                           65 00 50 00 61 00 64 00                           e.P.a.d.
```

### HID Report Descriptor

```c
0x05, 0x01,        // Usage Page (Generic Desktop Ctrls)
0x09, 0x05,        // Usage (Game Pad)
0xA1, 0x01,        // Collection (Application)
0x15, 0x00,        //   Logical Minimum (0)
0x25, 0x01,        //   Logical Maximum (1)
0x35, 0x00,        //   Physical Minimum (0)
0x45, 0x01,        //   Physical Maximum (1)
0x75, 0x01,        //   Report Size (1)
0x95, 0x0D,        //   Report Count (13)
0x05, 0x09,        //   Usage Page (Button)
0x19, 0x01,        //   Usage Minimum (0x01)
0x29, 0x0D,        //   Usage Maximum (0x0D)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x95, 0x03,        //   Report Count (3)
0x81, 0x01,        //   Input (Const,Array,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x01,        //   Usage Page (Generic Desktop Ctrls)
0x25, 0x07,        //   Logical Maximum (7)
0x46, 0x3B, 0x01,  //   Physical Maximum (315)
0x75, 0x04,        //   Report Size (4)
0x95, 0x01,        //   Report Count (1)
0x65, 0x14,        //   Unit (System: English Rotation, Length: Centimeter)
0x09, 0x39,        //   Usage (Hat switch)
0x81, 0x42,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State)
0x65, 0x00,        //   Unit (None)
0x95, 0x01,        //   Report Count (1)
0x81, 0x01,        //   Input (Const,Array,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x26, 0xFF, 0x00,  //   Logical Maximum (255)
0x46, 0xFF, 0x00,  //   Physical Maximum (255)
0x09, 0x30,        //   Usage (X)
0x09, 0x31,        //   Usage (Y)
0x09, 0x32,        //   Usage (Z)
0x09, 0x35,        //   Usage (Rz)
0x75, 0x08,        //   Report Size (8)
0x95, 0x04,        //   Report Count (4)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x06, 0x00, 0xFF,  //   Usage Page (Vendor Defined 0xFF00)
0x09, 0x20,        //   Usage (0x20)
0x09, 0x21,        //   Usage (0x21)
0x09, 0x22,        //   Usage (0x22)
0x09, 0x23,        //   Usage (0x23)
0x09, 0x24,        //   Usage (0x24)
0x09, 0x25,        //   Usage (0x25)
0x09, 0x26,        //   Usage (0x26)
0x09, 0x27,        //   Usage (0x27)
0x09, 0x28,        //   Usage (0x28)
0x09, 0x29,        //   Usage (0x29)
0x09, 0x2A,        //   Usage (0x2A)
0x09, 0x2B,        //   Usage (0x2B)
0x95, 0x0C,        //   Report Count (12)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x0A, 0x21, 0x26,  //   Usage (0x2621)
0x95, 0x08,        //   Report Count (8)
0xB1, 0x02,        //   Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x0A, 0x21, 0x26,  //   Usage (0x2621)
0x91, 0x02,        //   Output (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x26, 0xFF, 0x03,  //   Logical Maximum (1023)
0x46, 0xFF, 0x03,  //   Physical Maximum (1023)
0x09, 0x2C,        //   Usage (0x2C)
0x09, 0x2D,        //   Usage (0x2D)
0x09, 0x2E,        //   Usage (0x2E)
0x09, 0x2F,        //   Usage (0x2F)
0x75, 0x10,        //   Report Size (16)
0x95, 0x04,        //   Report Count (4)
0x81, 0x02,        //   Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0xC0,              // End Collection

// 137 bytes
```

## DualShock 4 (Wireless Controller) mode

### USBTreeViewer

```text

    =========================== USB Port6 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 7-6
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path              : \\?\usb#vid_054c&pid_05c4#8&1265ce96&0&6#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_054C&PID_05C4\8&1265CE96&0&6
Hardware IDs             : USB\VID_054C&PID_05C4&REV_0221 USB\VID_054C&PID_05C4
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0078 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.19041.3636  Date: 2023-10-26)
Driver Inf               : C:\WINDOWS\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0006.Hub_#0003
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(6), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP1)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT6)
Container ID             : {f59efcd4-1f3d-11ef-9546-d2d3cd0f52ac}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
EnhancedPowerMgmtEnabled : 1
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : HID-compliant game controller
  Device ID              : HID\VID_054C&PID_05C4\9&5B64A8E&5&0000
  Class                  : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags
 GlobalDisableSerNumGen  : REG_BINARY 00
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\054C05C40221
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x06 (6)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x03 (3)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt
Pipe[1]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 06 00 00 00 12 01 00 02 00 00 00 40 4C 05 C4 05   ...........@L...
                           21 02 01 02 00 01 01 01 00 03 00 02 00 00 00 01   !...............
                           00 00 00 07 05 81 03 40 00 05 00 00 00 00 07 05   .......@........
                           02 03 40 00 05 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x06 (6)
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
Data (HexDump)           : 06 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.00)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x054C (Sony Corporation)
idProduct                : 0x05C4
bcdDevice                : 0x0221
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Sony Computer Entertainment"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Wireless Controller"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 40 4C 05 C4 05 21 02 01 02   .......@L...!...
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0029 (41 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xC0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x01 (yes)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 02 29 00 01 01 00 C0 FA 09 04 00 00 02 03 00   ..).............
                           00 00 09 21 11 01 00 01 22 D3 01 07 05 81 03 40   ...!...."......@
                           00 05 07 05 02 03 40 00 05                        ......@..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
bAlternateSetting        : 0x00
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0x03 (HID - Human Interface Device)
bInterfaceSubClass       : 0x00 (None)
bInterfaceProtocol       : 0x00 (None)
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 00 02 03 00 00 00                        .........

        ------------------- HID Descriptor --------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x21 (HID Descriptor)
bcdHID                   : 0x0111 (HID Version 1.11)
bCountryCode             : 0x00 (00 = not localized)
bNumDescriptors          : 0x01
Data (HexDump)           : 09 21 11 01 00 01 22 D3 01                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x01D3 (467 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x05 (5 ms)
Data (HexDump)           : 07 05 81 03 40 00 05                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x05 (5 ms)
Data (HexDump)           : 07 05 02 03 40 00 05                              ....@..

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x38 (56 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Sony Computer Entertainment"
Data (HexDump)           : 38 03 53 00 6F 00 6E 00 79 00 20 00 43 00 6F 00   8.S.o.n.y. .C.o.
                           6D 00 70 00 75 00 74 00 65 00 72 00 20 00 45 00   m.p.u.t.e.r. .E.
                           6E 00 74 00 65 00 72 00 74 00 61 00 69 00 6E 00   n.t.e.r.t.a.i.n.
                           6D 00 65 00 6E 00 74 00                           m.e.n.t.
             ------ String Descriptor 2 ------
bLength                  : 0x28 (40 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Wireless Controller"
Data (HexDump)           : 28 03 57 00 69 00 72 00 65 00 6C 00 65 00 73 00   (.W.i.r.e.l.e.s.
                           73 00 20 00 43 00 6F 00 6E 00 74 00 72 00 6F 00   s. .C.o.n.t.r.o.
                           6C 00 6C 00 65 00 72 00                           l.l.e.r.

```
