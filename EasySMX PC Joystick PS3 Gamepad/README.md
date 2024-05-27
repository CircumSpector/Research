# EasySMX PC Joystick PS3 Gamepad

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
Device Description       : Xbox 360 Controller for Windows
Device Path              : \\?\usb#vid_2f24&pid_00ba#692918c80000#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_2F24&PID_00BA\692918C80000
Hardware IDs             : USB\VID_2F24&PID_00BA&REV_0100 USB\VID_2F24&PID_00BA
Driver KeyName           : {d61ca365-5af4-4486-998b-9db4734c6ca3}\0004 ({D61CA365-5AF4-4486-998B-9DB4734C6CA3})
Driver                   : \SystemRoot\System32\drivers\xusb22.sys (Version: 10.0.19041.4355  Date: 2024-05-15)
Driver Inf               : C:\WINDOWS\inf\xusb22.inf
Legacy BusType           : PNPBus
Class                    : XnaComposite
Class GUID               : {d61ca365-5af4-4486-998b-9db4734c6ca3}
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : xusb22
Enumerator               : USB
Location Info            : Port_#0006.Hub_#0003
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(6), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP1)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT6)
Container ID             : {b3a98b97-1378-582a-a968-6fe9d37e3197}
Manufacturer Info        : Microsoft
Capabilities             : 0x94 (Removable, UniqueID, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : USB Input Device
  Device ID              : USB\VID_2F24&PID_00BA&IG_00\9&DDABFE2&0&00
  Class                  : HIDClass
   Child Device 1        : HID-compliant game controller
    Device ID            : HID\VID_2F24&PID_00BA&IG_00\A&3366956B&0&0000
    Class                : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags
 GlobalDisableSerNumGen  : REG_BINARY 00
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\2F2400BA0100
 osvc                    : REG_BINARY 01 90
 SkipContainerIdQuery    : REG_BINARY 01 00

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
Data (HexDump)           : 06 00 00 00 12 01 00 02 FF FF FF 40 24 2F BA 00   ...........@$/..
                           00 01 01 02 03 01 01 01 00 03 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 40 00 04 00 00 00 00 07 05   .......@........
                           02 03 40 00 08 00 00 00 00                        ..@......

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
bDeviceClass             : 0xFF (Vendor Specific)
bDeviceSubClass          : 0xFF
bDeviceProtocol          : 0xFF
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x2F24
idProduct                : 0x00BA
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "  "
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "ESM GAME FOR WINDOWS 1.07"
iSerialNumber            : 0x03 (String Descriptor 3)
 Language 0x0409         : "692918C80000"
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 FF FF FF 40 24 2F BA 00 00 01 01 02   .......@$/......
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
                           08 00 00 07 05 81 03 40 00 04 07 05 02 03 40 00   .......@......@.
                           08                                                .

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
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
Data (HexDump)           : 11 21 00 01 01 25 81 14 00 00 00 00 13 02 08 00 
                           00 

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
Error                    : ERROR_GEN_FAILURE

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x06 (6 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "  "  *!*CAUTION  contains space characters only
Data (HexDump)           : 06 03 20 00 20 00                                 .. . .
             ------ String Descriptor 2 ------
bLength                  : 0x34 (52 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "ESM GAME FOR WINDOWS 1.07"
Data (HexDump)           : 34 03 45 00 53 00 4D 00 20 00 47 00 41 00 4D 00   4.E.S.M. .G.A.M.
                           45 00 20 00 46 00 4F 00 52 00 20 00 57 00 49 00   E. .F.O.R. .W.I.
                           4E 00 44 00 4F 00 57 00 53 00 20 00 31 00 2E 00   N.D.O.W.S. .1...
                           30 00 37 00                                       0.7.
             ------ String Descriptor 3 ------
bLength                  : 0x1A (26 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "692918C80000"
Data (HexDump)           : 1A 03 36 00 39 00 32 00 39 00 31 00 38 00 43 00   ..6.9.2.9.1.8.C.
                           38 00 30 00 30 00 30 00 30 00                     8.0.0.0.0.
             -- MSFT String Descriptor 0xEE --
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x03 (String Descriptor)
qwSignature Lang 0x0409  : "MSFT100"
bMS_VendorCode           : 0x90 (GET_MS_DESCRIPTOR=0x90)
bPad                     : 0x00
Data (HexDump)           : 12 03 4D 00 53 00 46 00 54 00 31 00 30 00 30 00   ..M.S.F.T.1.0.0.
                           90 00                                             ..
```
