# Microsoft Xbox One Controller

TBD

## UsbTreeView

```text

    =========================== USB Port9 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 1-9
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no
ConnectionIndex          : 9
CompanionIndex           : 0
 CompanionHubSymLnk      : USB#ROOT_HUB30#4&12dbcda0&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
 CompanionPortNumber     : 22

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : Xbox Controller
Device Path              : \\?\usb#vid_045e&pid_0b12#3039373132333036373234303430#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_045E&PID_0B12\3039373132333036373234303430
Hardware IDs             : USB\VID_045E&PID_0B12&REV_0515 USB\VID_045E&PID_0B12
Driver KeyName           : {05f5cfe2-4733-4950-a6bb-07aad01a3a84}\0000 ({05F5CFE2-4733-4950-A6BB-07AAD01A3A84})
Driver                   : \SystemRoot\System32\drivers\dc1-controller.sys (Version: 1.0.0.1  Date: 2024-05-17)
Driver Inf               : C:\WINDOWS\inf\dc1-controller.inf
Legacy BusType           : PNPBus
Class                    : XboxComposite
Class GUID               : {05f5cfe2-4733-4950-a6bb-07aad01a3a84}
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : dc1-controller
Enumerator               : USB
Location Info            : Port_#0009.Hub_#0001
Location IDs             : PCIROOT(0)#PCI(1400)#USBROOT(0)#USB(9), ACPI(_SB_)#ACPI(PCI0)#ACPI(XHC_)#ACPI(RHUB)#ACPI(HS09)
Container ID             : {a07b035e-586d-528e-bf2d-b7720ee4b73f}
Manufacturer Info        : Microsoft
Capabilities             : 0x94 (Removable, UniqueID, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Upper Filters            : xboxgip
IdleInWorkingState       : 1
WakeFromSleepState       : 1
Power State              : D0 (supported: D0, D1, D2, D3, wake from D0, wake from D1, wake from D2)
 Child Device 1          : USB Input Device
  Device ID              : USB\VID_045E&PID_02FF&IG_00\00&00&0000C9D46A86ED7E
  Class                  : HIDClass
   Child Device 1        : XINPUT compatible HID device
    Device ID            : HID\VID_045E&PID_02FF&IG_00\7&1E0D48F8&1&0000
    Class                : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags
 GlobalDisableSerNumGen  : REG_BINARY 00
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\045E0B120515
 osvc                    : REG_BINARY 01 90
 SkipContainerIdQuery    : REG_BINARY 01 00

        ---------------- Connection Information ---------------
Connection Index         : 0x09 (9)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x19 (25)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt
Pipe[1]                  : EndpointID=2  Direction=IN   ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 09 00 00 00 12 01 00 02 FF 47 D0 40 5E 04 12 0B   .........G.@^...
                           15 05 01 02 03 01 01 01 00 19 00 02 00 00 00 01   ................
                           00 00 00 07 05 02 03 40 00 04 00 00 00 00 07 05   .......@........
                           82 03 40 00 02 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x09 (9)
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
Data (HexDump)           : 09 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.00)
bDeviceClass             : 0xFF (Vendor Specific)
bDeviceSubClass          : 0x47
bDeviceProtocol          : 0xD0
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x045E (Microsoft Corporation)
idProduct                : 0x0B12
bcdDevice                : 0x0515
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Microsoft"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Controller"
iSerialNumber            : 0x03 (String Descriptor 3)
 Language 0x0409         : "3039373132333036373234303430"
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 FF 47 D0 40 5E 04 12 0B 15 05 01 02   .....G.@^.......
                           03 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0077 (119 bytes)
bNumInterfaces           : 0x03 (3 Interfaces)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xA0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x01 (yes)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 02 77 00 03 01 00 A0 FA 09 04 00 00 02 FF 47   ..w............G
                           D0 00 07 05 02 03 40 00 04 07 05 82 03 40 00 04   ......@......@..
                           09 04 00 01 02 FF 47 D0 00 07 05 02 03 40 00 04   ......G......@..
                           07 05 82 03 40 00 02 09 04 01 00 00 FF 47 D0 00   ....@........G..
                           09 04 01 01 02 FF 47 D0 00 07 05 03 01 E4 00 01   ......G.........
                           07 05 83 01 40 00 01 09 04 02 00 00 FF 47 D0 00   ....@........G..
                           09 04 02 01 02 FF 47 D0 00 07 05 04 02 40 00 00   ......G......@..
                           07 05 84 02 40 00 00                              ....@..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
bAlternateSetting        : 0x00
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x47
bInterfaceProtocol       : 0xD0
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 00 02 FF 47 D0 00                        ......G..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 02 03 40 00 04                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x82 (Direction=IN EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 82 03 40 00 04                              ....@..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
bAlternateSetting        : 0x01
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x47
bInterfaceProtocol       : 0xD0
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 01 02 FF 47 D0 00                        ......G..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 02 03 40 00 04                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x82 (Direction=IN EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x02 (2 ms)
Data (HexDump)           : 07 05 82 03 40 00 02                              ....@..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x01
bAlternateSetting        : 0x00
bNumEndpoints            : 0x00 (Default Control Pipe only)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x47
bInterfaceProtocol       : 0xD0
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 01 00 00 FF 47 D0 00                        ......G..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x01
bAlternateSetting        : 0x01
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x47
bInterfaceProtocol       : 0xD0
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 01 01 02 FF 47 D0 00                        ......G..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x03 (Direction=OUT EndpointID=3)
bmAttributes             : 0x01 (TransferType=Isochronous  SyncType=None  EndpointType=Data)
wMaxPacketSize           : 0x00E4 (228 bytes)
bInterval                : 0x01 (125 µs)
Data (HexDump)           : 07 05 03 01 E4 00 01                              .......

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x83 (Direction=IN EndpointID=3)
bmAttributes             : 0x01 (TransferType=Isochronous  SyncType=None  EndpointType=Data)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x01 (125 µs)
Data (HexDump)           : 07 05 83 01 40 00 01                              ....@..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x02
bAlternateSetting        : 0x00
bNumEndpoints            : 0x00 (Default Control Pipe only)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x47
bInterfaceProtocol       : 0xD0
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 02 00 00 FF 47 D0 00                        ......G..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x02
bAlternateSetting        : 0x01
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0xFF (Vendor Specific)
bInterfaceSubClass       : 0x47
bInterfaceProtocol       : 0xD0
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 02 01 02 FF 47 D0 00                        ......G..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x04 (Direction=OUT EndpointID=4)
bmAttributes             : 0x02 (TransferType=Bulk)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x00 (ignored)
Data (HexDump)           : 07 05 04 02 40 00 00                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x84 (Direction=IN EndpointID=4)
bmAttributes             : 0x02 (TransferType=Bulk)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x00 (ignored)
Data (HexDump)           : 07 05 84 02 40 00 00                              ....@..

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x14 (20 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Microsoft"
Data (HexDump)           : 14 03 4D 00 69 00 63 00 72 00 6F 00 73 00 6F 00   ..M.i.c.r.o.s.o.
                           66 00 74 00                                       f.t.
             ------ String Descriptor 2 ------
bLength                  : 0x16 (22 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Controller"
Data (HexDump)           : 16 03 43 00 6F 00 6E 00 74 00 72 00 6F 00 6C 00   ..C.o.n.t.r.o.l.
                           6C 00 65 00 72 00                                 l.e.r.
             ------ String Descriptor 3 ------
bLength                  : 0x3A (58 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "3039373132333036373234303430"
Data (HexDump)           : 3A 03 33 00 30 00 33 00 39 00 33 00 37 00 33 00   :.3.0.3.9.3.7.3.
                           31 00 33 00 32 00 33 00 33 00 33 00 30 00 33 00   1.3.2.3.3.3.0.3.
                           36 00 33 00 37 00 33 00 32 00 33 00 34 00 33 00   6.3.7.3.2.3.4.3.
                           30 00 33 00 34 00 33 00 30 00                     0.3.4.3.0.
             -- MSFT String Descriptor 0xEE --
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x03 (String Descriptor)
qwSignature Lang 0x0409  : "MSFT100"
bMS_VendorCode           : 0x90 (GET_MS_DESCRIPTOR=0x90)
bPad                     : 0x00
Data (HexDump)           : 12 03 4D 00 53 00 46 00 54 00 31 00 30 00 30 00   ..M.S.F.T.1.0.0.
                           90 00                                             ..
```

## Wireshark filter

```text
(((((((((((!(usbll.pid == 0xd2)) && !(usbll.pid == 0xa5)) && !(usbll.pid == 0x5a)) && !(usbll.pid == 0x69)) && !(usbll.pid == 0x65)) && !(usbll.pid == 0xd9)) && !(usbll.pid == 0xb2)) && !(usbll.pid == 0xc7)) && !(usbll.pid == 0x77)) && !(usbll.pid == 0xcb)) && !(usbll.pid == 0xcf)) && !(usbll.pid == 0xb7)
```
