# Retro Fighters Defender

To be done...

```text
Device Description: USB Input Device
Hardware Ids: USB\VID_2563&PID_0575&REV_0100  & USB\VID_2563&PID_0575
Display Name: Human Interface Devices
Physical Device Object Name: \Device\USBPDO-3
Class Guid: {745a17a0-74d3-11d0-b6fe-00a0c90f57da}
Driver Key: {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0645
Device Instance Path: USB\VID_2563&PID_0575\12
Class: HIDClass
Inf Name: input.inf
Children: HID\VID_2563&PID_0575\6&266ff556&1&0000
Reported Device Ids Hash: AFCF5503
```

```
  1. Triangle
    2. Circle
    3. Cross
    4. Square
    5. Up
    6. Right
    7. Down
    8. Left
    9. R1
    10. L1
```

## XInput Mode (Default)

### USBTreeView

```text

    =========================== USB Port8 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 2-8

      ========================== Summary =========================
Vendor ID                : 0x045E (Microsoft Corporation)
Product ID               : 0x028E
USB Version              : 1.1
Port maximum Speed       : High-Speed
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : no
Demanded Current         : 500 mA
Used Endpoints           : 3

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : Xbox 360 Controller for Windows
Device Path 1            : \\?\USB#VID_045E&PID_028E#10F36D6#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Device Path 2            : \\?\USB#VID_045E&PID_028E#10F36D6#{ec87f1e3-c13b-4100-b5f7-8b84d54260cb}
Device Path 3            : \\?\USB#VID_045E&PID_028E#10F36D6#{86431f5b-9f5a-48ce-8fbf-a537413ef358}
Kernel Name              : \Device\USBPDO-10
Device ID                : USB\VID_045E&PID_028E\10F36D6
Hardware IDs             : USB\VID_045E&PID_028E&REV_0110 USB\VID_045E&PID_028E
Driver KeyName           : {d61ca365-5af4-4486-998b-9db4734c6ca3}\0008
Driver                   : \SystemRoot\System32\drivers\xusb22.sys (Version: 10.0.19041.1  Date: 2019-12-07)
Driver Inf               : C:\WINDOWS\inf\xusb22.inf
Legacy BusType           : PNPBus
Class                    : XnaComposite
Class GUID               : {d61ca365-5af4-4486-998b-9db4734c6ca3}
Service                  : xusb22
Enumerator               : USB
Location Info            : Port_#0008.Hub_#0001
Location IDs             : PCIROOT(0)#PCI(1400)#USBROOT(0)#USB(8), ACPI(_SB_)#ACPI(PCI0)#ACPI(XHC_)#ACPI(RHUB)#ACPI(HS08)
Container ID             : {b562bbc7-1756-52f5-906d-740400fe2902}
Manufacturer Info        : Microsoft
Capabilities             : 0x94 (Removable, UniqueID, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
HcDisableSelectiveSuspend: 0
EnableSelectiveSuspend   : 0
SelectiveSuspendEnabled  : 0
EnhancedPowerMgmtEnabled : 0
IdleInWorkingState       : 0
WakeFromSleepState       : 0
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : USB Input Device
  Device ID              : USB\VID_045E&PID_028E&IG_00\6&1E86ACC6&0&00
  Class                  : HIDClass
  Driver KeyName         : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0064 (GUID_DEVCLASS_HIDCLASS)
  Service                : HidUsb
  Location               : XBOX_360_DEVICE_00:00
   Child Device 1        : HID-compliant game controller
    Device Path 1        : \\?\HID#VID_045E&PID_028E&IG_00#7&19f79548&0&0000#{86431f5b-9f5a-48ce-8fbf-a537413ef358}
    Device Path 2        : \\?\HID#VID_045E&PID_028E&IG_00#7&19f79548&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030} (GUID_DEVINTERFACE_HID)
    Kernel Name          : \Device\000000b4
    Device ID            : HID\VID_045E&PID_028E&IG_00\7&19F79548&0&0000
    Class                : HIDClass
    Driver KeyName       : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0065 (GUID_DEVCLASS_HIDCLASS)

        ---------------- Connection Information ---------------
Connection Index         : 0x08 (Port 8)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x1E (30)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=32    bInterval=8
Pipe[1]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=32    bInterval=8
Data (HexDump)           : 08 00 00 00 12 01 10 01 FF FF FF 40 5E 04 8E 02   ...........@^...
                           10 01 01 02 03 01 01 01 00 1E 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 20 00 08 00 00 00 00 07 05   ....... ........
                           02 03 20 00 08 00 00 00 00                        .. ......

        --------------- Connection Information V2 -------------
Connection Index         : 0x08 (8)
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
Data (HexDump)           : 08 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

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
 Language 0x0409         : "ShanWan"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Retro Fͩghters ͇amepad"
iSerialNumber            : 0x03 (String Descriptor 3)
 Language 0x0409         : "10F36D6"
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

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x10 (16 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "ShanWan"
Data (HexDump)           : 10 03 53 00 68 00 61 00 6E 00 57 00 61 00 6E 00   ..S.h.a.n.W.a.n.
             ------ String Descriptor 2 ------
bLength                  : 0x2E (46 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Retro Fͩghters ͇amepad"
Data (HexDump)           : 2E 03 52 00 65 00 74 00 72 00 6F 00 20 00 46 00   ..R.e.t.r.o. .F.
                           69 03 67 00 68 00 74 00 65 00 72 00 73 00 20 00   i.g.h.t.e.r.s. .
                           47 03 61 00 6D 00 65 00 70 00 61 00 64 00         G.a.m.e.p.a.d.
             ------ String Descriptor 3 ------
bLength                  : 0x10 (16 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "10F36D6"
Data (HexDump)           : 10 03 31 00 30 00 46 00 33 00 36 00 44 00 36 00   ..1.0.F.3.6.D.6.
```

## DirectInput Mode (Analogue)

### USBTreeView

```text

    =========================== USB Port4 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 4-4
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no
ConnectionIndex          : 4
CompanionIndex           : 0
 CompanionHubSymLnk      : USB#ROOT_HUB30#7&37c7c63c&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
 CompanionPortNumber     : 10

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path              : \\?\usb#vid_2563&pid_0575#8&1265ce96&0&4#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_2563&PID_0575\8&1265CE96&0&4
Hardware IDs             : USB\VID_2563&PID_0575&REV_0100 USB\VID_2563&PID_0575
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0033 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.19041.868  Date: 2021-04-18)
Driver Inf               : C:\WINDOWS\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0004.Hub_#0002
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(4), ACPI(_SB_)#ACPI(PCI0)#ACPI(BXBR)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT4)
Container ID             : {79629f79-55dc-11ed-9457-ca74e3e6ad6c}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
EnhancedPowerMgmtEnabled : 1
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : HID-compliant game controller
  Device ID              : HID\VID_2563&PID_0575\9&2F3C6796&0&0000
  Class                  : HIDClass

        ---------------- Connection Information ---------------
Connection Index         : 0x04 (4)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x03 (3)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=2  Direction=OUT  ScheduleOffset=0  Type=Interrupt
Pipe[1]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 04 00 00 00 12 01 10 01 00 00 00 40 63 25 75 05   ...........@c%u.
                           00 01 01 02 00 01 01 01 00 03 00 02 00 00 00 01   ................
                           00 00 00 07 05 02 03 40 00 0A 00 00 00 00 07 05   .......@........
                           81 03 40 00 0A 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x04 (4)
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
Data (HexDump)           : 04 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x110 (USB Version 1.10)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x2563
idProduct                : 0x0575
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 *!*ERROR  String descriptor not found
iProduct                 : 0x02 (String Descriptor 2)
 *!*ERROR  String descriptor not found
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
                           00 0A 07 05 81 03 40 00 0A                        ......@..

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
Data (HexDump)           : 09 21 11 01 00 01 22 89 00                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0089 (137 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 02 03 40 00 0A                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 81 03 40 00 0A                              ....@..

      -------------------- String Descriptors -------------------
none

```

## DirectInput Mode (Digital)

### USBTreeView

```text

    =========================== USB Port8 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 2-8

      ========================== Summary =========================
Vendor ID                : 0x054C (Sony Group Corporation)
Product ID               : 0x0CDA
USB Version              : 2.0 -> but Device is Full-Speed only
Port maximum Speed       : High-Speed
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : no
Demanded Current         : 100 mA
Used Endpoints           : 2

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path 1            : \\?\USB#VID_054C&PID_0CDA#5&1ece9816&0&8#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Device Path 2            : \\?\USB#VID_054C&PID_0CDA#5&1ece9816&0&8#{86431f5b-9f5a-48ce-8fbf-a537413ef358}
Kernel Name              : \Device\USBPDO-10
Device ID                : USB\VID_054C&PID_0CDA\5&1ECE9816&0&8
Hardware IDs             : USB\VID_054C&PID_0CDA&REV_0100 USB\VID_054C&PID_0CDA
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0070 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.19041.868  Date: 2021-04-30)
Driver Inf               : C:\WINDOWS\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0008.Hub_#0001
Location IDs             : PCIROOT(0)#PCI(1400)#USBROOT(0)#USB(8), ACPI(_SB_)#ACPI(PCI0)#ACPI(XHC_)#ACPI(RHUB)#ACPI(HS08)
Container ID             : {f333f586-52df-11ed-9bc4-bcca40012580}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
HcDisableSelectiveSuspend: 0
EnableSelectiveSuspend   : 0
SelectiveSuspendEnabled  : 0
EnhancedPowerMgmtEnabled : 1
IdleInWorkingState       : 0
WakeFromSleepState       : 0
Power State              : D0 (supported: D0, D1, D2, D3, wake from D0, wake from D1, wake from D2)
 Child Device 1          : HID-compliant game controller
  Device Path 1          : \\?\HID#VID_054C&PID_0CDA#6&344fd1cb&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030} (GUID_DEVINTERFACE_HID)
  Device Path 2          : \\?\HID#VID_054C&PID_0CDA#6&344fd1cb&0&0000#{86431f5b-9f5a-48ce-8fbf-a537413ef358}
  Kernel Name            : \Device\000000b6
  Device ID              : HID\VID_054C&PID_0CDA\6&344FD1CB&0&0000
  Class                  : HIDClass
  Driver KeyName         : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0071 (GUID_DEVCLASS_HIDCLASS)

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\054C0CDA0100
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x08 (Port 8)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x20 (32)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x01 (1 pipe to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=64    bInterval=10
Data (HexDump)           : 08 00 00 00 12 01 00 02 00 00 00 40 4C 05 DA 0C   ...........@L...
                           00 01 01 02 00 01 01 01 00 20 00 01 00 00 00 01   ......... ......
                           00 00 00 07 05 81 03 40 00 0A 00 00 00 00         .......@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x08 (8)
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
Data (HexDump)           : 08 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.0) -> but device is Full-Speed only
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x054C (Sony Group Corporation)
idProduct                : 0x0CDA
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Sony Interactive Entertainment"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Controller"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 40 4C 05 DA 0C 00 01 01 02   .......@L.......
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0022 (34 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xA0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x01 (yes)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0x32 (100 mA)
Data (HexDump)           : 09 02 22 00 01 01 00 A0 32 09 04 00 00 01 03 00   ..".....2.......
                           00 00 09 21 11 01 00 01 22 31 00 07 05 81 03 40   ...!...."1.....@
                           00 0A                                             ..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00 (Interface 0)
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
Data (HexDump)           : 09 21 11 01 00 01 22 31 00                        .!...."1.
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0031 (49 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER (due to a obscure limitation of the Win32 USB API, see UsbTreeView.txt)

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 81 03 40 00 0A                              ....@..

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE  (because the device is Full-Speed only)

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x3E (62 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Sony Interactive Entertainment"
Data (HexDump)           : 3E 03 53 00 6F 00 6E 00 79 00 20 00 49 00 6E 00   >.S.o.n.y. .I.n.
                           74 00 65 00 72 00 61 00 63 00 74 00 69 00 76 00   t.e.r.a.c.t.i.v.
                           65 00 20 00 45 00 6E 00 74 00 65 00 72 00 74 00   e. .E.n.t.e.r.t.
                           61 00 69 00 6E 00 6D 00 65 00 6E 00 74 00         a.i.n.m.e.n.t.
             ------ String Descriptor 2 ------
bLength                  : 0x16 (22 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Controller"
Data (HexDump)           : 16 03 43 00 6F 00 6E 00 74 00 72 00 6F 00 6C 00   ..C.o.n.t.r.o.l.
                           6C 00 65 00 72 00                                 l.e.r.

```
