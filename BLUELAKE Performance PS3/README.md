# BLUELAKE Performance PS3

- Works with DsHidMini
  - Wired
  - Wireless except LEDs

TBD

## Windows

### USBTreeView

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
Friendly Name            : USB Gamepad
Device Description       : DS3 Compatible HID Device
Device Path              : \\?\usb#vid_054c&pid_0268#8&1265ce96&0&6#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_054C&PID_0268\8&1265CE96&0&6
Hardware IDs             : USB\VID_054C&PID_0268&REV_0100 USB\VID_054C&PID_0268
Driver KeyName           : {2b959c9d-a4ed-4464-809d-0f1118cf055d}\0000 ({2B959C9D-A4ED-4464-809D-0F1118CF055D})
Driver                   : \SystemRoot\System32\drivers\mshidumdf.sys (Version: 10.0.19041.1  Date: 2019-12-07)
Driver Inf               : C:\WINDOWS\inf\oem67.inf
Legacy BusType           : PNPBus
Class                    : Nefarius HID Devices
Class GUID               : {2b959c9d-a4ed-4464-809d-0f1118cf055d}
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : mshidumdf
Enumerator               : USB
Location Info            : Port_#0006.Hub_#0003
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(6), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP1)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT6)
Container ID             : {cc3aa18e-0421-11ef-953f-f13b721d0e15}
Manufacturer Info        : Nefarius Software Solutions e.U.
Capabilities             : 0x04 (Removable)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Lower Filters            : WUDFRd, nssmkig
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : HID-compliant game controller
  DevicePath             : \\?\hid#vid_054c&pid_0268#9&69fdf83&2&0000#{4d1e55b2-f16f-11cf-88cb-001111000030}
  KernelName             : \Device\0000039d
  Device ID              : HID\VID_054C&PID_0268\9&69FDF83&2&0000
  Class                  : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags
 GlobalDisableSerNumGen  : REG_BINARY 00
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\054C02680100
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
Data (HexDump)           : 06 00 00 00 12 01 00 02 00 00 00 40 4C 05 68 02   ...........@L.h.
                           00 01 01 02 00 01 01 01 00 03 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 40 00 0A 00 00 00 00 07 05   .......@........
                           02 03 40 00 0A 00 00 00 00                        ..@......

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
idProduct                : 0x0268
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Nintendo Co., Ltd."
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "USB Gamepad"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 40 4C 05 68 02 00 01 01 02   .......@L.h.....
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
                           00 00 09 21 10 01 00 01 22 94 00 07 05 81 03 40   ...!...."......@
                           00 0A 07 05 02 03 40 00 0A                        ......@..

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
bcdHID                   : 0x0110 (HID Version 1.10)
bCountryCode             : 0x00 (00 = not localized)
bNumDescriptors          : 0x01
Data (HexDump)           : 09 21 10 01 00 01 22 94 00                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0094 (148 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 81 03 40 00 0A                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x02 (Direction=OUT EndpointID=2)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 02 03 40 00 0A                              ....@..

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x26 (38 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Nintendo Co., Ltd."
Data (HexDump)           : 26 03 4E 00 69 00 6E 00 74 00 65 00 6E 00 64 00   &.N.i.n.t.e.n.d.
                           6F 00 20 00 43 00 6F 00 2E 00 2C 00 20 00 4C 00   o. .C.o...,. .L.
                           74 00 64 00 2E 00                                 t.d...
             ------ String Descriptor 2 ------
bLength                  : 0x18 (24 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "USB Gamepad"
Data (HexDump)           : 18 03 55 00 53 00 42 00 20 00 47 00 61 00 6D 00   ..U.S.B. .G.a.m.
                           65 00 70 00 61 00 64 00                           e.p.a.d.
             ----- String Descriptor 0xEE -----
bLength                  : 0x28 (40 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Wireless Controller"
Data (HexDump)           : 28 03 57 00 69 00 72 00 65 00 6C 00 65 00 73 00   (.W.i.r.e.l.e.s.
                           73 00 20 00 43 00 6F 00 6E 00 74 00 72 00 6F 00   s. .C.o.n.t.r.o.
                           6C 00 6C 00 65 00 72 00                           l.l.e.r.
```
