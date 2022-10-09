# Collective Minds Strike Pack Eliminator Mod Pack - PlayStation 4

## Hardware IDs

```text
USB\VID_054C&PID_05C5&REV_0100
USB\VID_054C&PID_05C5
```

## USBTreeView

```text

    =========================== USB Port3 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 4-3
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no
ConnectionIndex          : 3
CompanionIndex           : 0
 CompanionHubSymLnk      : USB#ROOT_HUB30#7&37c7c63c&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
 CompanionPortNumber     : 9

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path              : \\?\usb#vid_054c&pid_05c5#8&1265ce96&0&3#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_054C&PID_05C5\8&1265CE96&0&3
Hardware IDs             : USB\VID_054C&PID_05C5&REV_0100 USB\VID_054C&PID_05C5
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0097 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.19041.868  Date: 2021-04-18)
Driver Inf               : C:\WINDOWS\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0003.Hub_#0002
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(3), ACPI(_SB_)#ACPI(PCI0)#ACPI(BXBR)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT3)
Container ID             : {fa9cee31-474c-11ed-9452-fd82f29fe66d}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
EnhancedPowerMgmtEnabled : 1
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : HID-compliant game controller
  DevicePath             : \\?\hid#vid_054c&pid_05c5&col01#9&15d29643&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030}
  KernelName             : \Device\000002fb
  Device ID              : HID\VID_054C&PID_05C5&COL01\9&15D29643&0&0000
  Class                  : HIDClass
 Child Device 2          : HID-compliant vendor-defined device
  DevicePath             : \\?\hid#vid_054c&pid_05c5&col02#9&15d29643&0&0001#{4d1e55b2-f16f-11cf-88cb-001111000030}
  KernelName             : \Device\000002fc
  Device ID              : HID\VID_054C&PID_05C5&COL02\9&15D29643&0&0001
  Class                  : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\054C05C50100
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x03 (3)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x03 (3)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt
Pipe[1]                  : EndpointID=1  Direction=OUT  ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 03 00 00 00 12 01 00 02 00 00 00 40 4C 05 C5 05   ...........@L...
                           00 01 01 02 00 01 01 01 00 03 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 40 00 01 00 00 00 00 07 05   .......@........
                           01 03 40 00 05 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x03 (3)
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
Data (HexDump)           : 03 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.00)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x054C (Sony Corporation)
idProduct                : 0x05C5
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Sony Computer Entertainment"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Wireless Controller"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 40 4C 05 C5 05 00 01 01 02   .......@L.......
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
                           00 00 09 21 11 01 00 01 22 CC 00 07 05 81 03 40   ...!...."......@
                           00 01 07 05 01 03 40 00 05                        ......@..

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
Data (HexDump)           : 09 21 11 01 00 01 22 CC 00                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x00CC (204 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x01 (1 ms)
Data (HexDump)           : 07 05 81 03 40 00 01                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x01 (Direction=OUT EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x05 (5 ms)
Data (HexDump)           : 07 05 01 03 40 00 05                              ....@..

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
