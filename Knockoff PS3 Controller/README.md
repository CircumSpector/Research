# Unknown Knockoff PS3 Controller

## Hardware IDs

USB
```text
HID\VID_045E&PID_028E&IG_00\A&32384F79&0&0000
```
BT
```text
HID\{00001124-0000-1000-8000-00805F9B34FB}_VID&0002054C_PID&09CC\C&31157879&12&0000
```

## USBTreeView

```text
=========================== USB Port9 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 2-9
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no
ConnectionIndex          : 0x09 (Port 9)
CompanionIndex           : 0
 CompanionHubSymLnk      : USB#ROOT_HUB30#7&27ed1eec&0&0#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
 CompanionPortNumber     : 0x03 (Port 3)
 -> CompanionPortChain   : 2-3

      ========================== Summary =========================
Vendor ID                : 0x045E (Microsoft Corporation)
Product ID               : 0x028E
USB Version              : 2.0 -> but Device is Full-Speed only
Port maximum Speed       : High-Speed (Companion Port 2-3 supports SuperSpeed)
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : no
Demanded Current         : 500 mA
Used Endpoints           : 3

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : Controlador XBOX 360 para Windows
Device Path 1            : \\?\USB#VID_045E&PID_028E#8&1199c2a1&0&9#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Device Path 2            : \\?\USB#VID_045E&PID_028E#8&1199c2a1&0&9#{ec87f1e3-c13b-4100-b5f7-8b84d54260cb}
Kernel Name              : \Device\USBPDO-7
Device ID                : USB\VID_045E&PID_028E\8&1199C2A1&0&9
Hardware IDs             : USB\VID_045E&PID_028E&REV_0110 USB\VID_045E&PID_028E
Driver KeyName           : {d61ca365-5af4-4486-998b-9db4734c6ca3}\0000
Driver                   : \SystemRoot\System32\drivers\xusb22.sys (Version: 10.0.22621.3085  Date: 2024-02-15  Company: Microsoft Corporation)
Driver Inf               : C:\Windows\inf\xusb22.inf
Legacy BusType           : PNPBus
Class                    : XnaComposite
Class GUID               : {d61ca365-5af4-4486-998b-9db4734c6ca3}
Service                  : xusb22
Enumerator               : USB
Location Info            : Port_#0009.Hub_#0005
Address                  : 9
Location IDs             : PCIROOT(0)#PCI(0201)#PCI(0000)#PCI(0C00)#PCI(0000)#USBROOT(0)#USB(9), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP7)#ACPI(UP00)#ACPI(DP60)#ACPI(XH00)#ACPI(RHUB)#ACPI(POT9)
Container ID             : {23bcff93-ceac-11ee-b6c6-106fd9d9e098}
Manufacturer Info        : Microsoft
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Power State              : D0 (supported: D0, D1, D2, D3, wake from D0, wake from D1, wake from D2)

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\045E028E0110
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x09 (Port 9)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x08 (8)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number of open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x20    bInterval=4   -> 420 Bits/ms = 52500 Bytes/s
Pipe[1]                  : EndpointID=1  Direction=OUT  ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x20    bInterval=8   -> 420 Bits/ms = 52500 Bytes/s
Data (HexDump)           : 09 00 00 00 12 01 00 02 FF FF FF 40 5E 04 8E 02   ...........@^...
                           10 01 01 02 00 01 01 01 00 08 00 02 00 00 00 01   ................
                           00 00 00 07 05 81 03 20 00 04 00 00 00 00 07 05   ....... ........
                           01 03 20 00 08 00 00 00 00                        .. ......

        --------------- Connection Information V2 -------------
Connection Index         : 0x09 (9)
Length                   : 0x10 (16 bytes)
SupportedUsbProtocols    : 0x03
 Usb110                  : 1 (yes, port supports USB 1.1)
 Usb200                  : 1 (yes, port supports USB 2.0)
 Usb300                  : 0 (no, port not supports USB 3.0) -> but Companion Port 2-3 does
 ReservedMBZ             : 0x00
Flags                    : 0x00
 DevIsOpAtSsOrHigher     : 0 (Device is not operating at SuperSpeed or higher)
 DevIsSsCapOrHigher      : 0 (Device is not SuperSpeed capable or higher)
 DevIsOpAtSsPlusOrHigher : 0 (Device is not operating at SuperSpeedPlus or higher)
 DevIsSsPlusCapOrHigher  : 0 (Device is not SuperSpeedPlus capable or higher)
 ReservedMBZ             : 0x00
Data (HexDump)           : 09 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.0) -> but device is Full-Speed only
bDeviceClass             : 0xFF (Vendor Specific)
bDeviceSubClass          : 0xFF
bDeviceProtocol          : 0xFF
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x045E (Microsoft Corporation)
idProduct                : 0x028E
bcdDevice                : 0x0110
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Sony"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Controller"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 FF FF FF 40 5E 04 8E 02 10 01 01 02   .......@^.......
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x0030 (48 bytes)
bNumInterfaces           : 0x01 (1 Interface)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xA0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x00 (no)
 D5: Remote Wakeup       : 0x01 (yes)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 02 30 00 01 01 00 A0 FA 09 04 00 00 02 FF 5D   ..0............]
                           01 00 10 21 10 01 01 24 81 14 03 00 03 13 01 08   ...!...$........
                           03 00 07 05 81 03 20 00 04 07 05 01 03 20 00 08   ...... ...... ..

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
Data (HexDump)           : 10 21 10 01 01 24 81 14 03 00 03 13 01 08 03 00 
                           
        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0020 (32 bytes)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 81 03 20 00 04                              .... ..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x01 (Direction=OUT EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0020 (32 bytes)
bInterval                : 0x08 (8 ms)
Data (HexDump)           : 07 05 01 03 20 00 08                              .... ..

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE  (because the device is Full-Speed only)

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 1 ------
bLength                  : 0x0A (10 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Sony"
Data (HexDump)           : 0A 03 53 00 6F 00 6E 00 79 00                     ..S.o.n.y.
             ------ String Descriptor 2 ------
bLength                  : 0x16 (22 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Controller"
Data (HexDump)           : 16 03 43 00 6F 00 6E 00 74 00 72 00 6F 00 6C 00   ..C.o.n.t.r.o.l.
                           6C 00 65 00 72 00                                 l.e.r.
```