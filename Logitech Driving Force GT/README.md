# Logitech Driving Force GT

## Hardware IDs

```text
USB\VID_046D&PID_C294&REV_1327
USB\VID_046D&PID_C294
```

## USBTreeView

```text

    =========================== USB Port10 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 3-10
Properties               : 0x01
 IsUserConnectable       : yes
 PortIsDebugCapable      : no
 PortHasMultiCompanions  : no
 PortConnectorIsTypeC    : no

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Input Device
Device Path              : \\?\usb#vid_046d&pid_c294#5&4330a47&2&10#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_046D&PID_C294\5&4330A47&2&10
Hardware IDs             : USB\VID_046D&PID_C294&REV_1327 USB\VID_046D&PID_C294
Driver KeyName           : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0040 (GUID_DEVCLASS_HIDCLASS)
Driver                   : \SystemRoot\System32\drivers\hidusb.sys (Version: 10.0.22621.819  Date: 2022-12-13)
Driver Inf               : C:\Windows\inf\input.inf
Legacy BusType           : PNPBus
Class                    : HIDClass
Class GUID               : {745a17a0-74d3-11d0-b6fe-00a0c90f57da} (GUID_DEVCLASS_HIDCLASS)
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : HidUsb
Enumerator               : USB
Location Info            : Port_#0010.Hub_#0001
Location IDs             : PCIROOT(0)#PCI(1400)#USBROOT(0)#USB(10), ACPI(_SB_)#ACPI(PCI0)#ACPI(XHC_)#ACPI(RHUB)#ACPI(HS10)
Container ID             : {ad1b823b-c1cd-11ed-9aff-480fcf488337}
Manufacturer Info        : (Standard system devices)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
EnhancedPowerMgmtEnabled : 1
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : HID-compliant game controller
  DevicePath             : \\?\hid#vid_046d&pid_c294#6&61101e2&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030}
  KernelName             : \Device\00000077
  Device ID              : HID\VID_046D&PID_C294\6&61101E2&0&0000
  Class                  : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\046DC2941327
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x0A (10)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x0C (12)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=1  Direction=IN   ScheduleOffset=0  Type=Interrupt
Pipe[1]                  : EndpointID=1  Direction=OUT  ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 0A 00 00 00 12 01 00 02 00 00 00 10 6D 04 94 C2   ............m...
                           27 13 00 02 00 01 01 01 00 0C 00 02 00 00 00 01   '...............
                           00 00 00 07 05 81 03 08 00 0A 00 00 00 00 07 05   ................
                           01 03 08 00 0A 00 00 00 00                        .........

        --------------- Connection Information V2 -------------
Connection Index         : 0x0A (10)
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
Data (HexDump)           : 0A 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.00)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x10 (16 bytes)
idVendor                 : 0x046D (Logitech Inc.)
idProduct                : 0xC294
bcdDevice                : 0x1327
iManufacturer            : 0x00 (No String Descriptor)
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Driving Force GT"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 10 6D 04 94 C2 27 13 00 02   ........m...'...
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
MaxPower                 : 0x28 (80 mA)
Data (HexDump)           : 09 02 29 00 01 01 00 80 28 09 04 00 00 02 03 00   ..).....(.......
                           00 00 09 21 00 01 21 01 22 89 00 07 05 81 03 08   ...!..!.".......
                           00 0A 07 05 01 03 08 00 0A                        .........

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
bcdHID                   : 0x0100 (HID Version 1.00)
bCountryCode             : 0x21 (33 = US)
bNumDescriptors          : 0x01
Data (HexDump)           : 09 21 00 01 21 01 22 89 00                        .!..!."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0089 (137 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x81 (Direction=IN EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0008 (8 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 81 03 08 00 0A                              .......

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x01 (Direction=OUT EndpointID=1)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0008 (8 bytes)
bInterval                : 0x0A (10 ms)
Data (HexDump)           : 07 05 01 03 08 00 0A                              .......

    ----------------- Device Qualifier Descriptor -----------------
Error                    : ERROR_GEN_FAILURE

      -------------------- String Descriptors -------------------
             ------ String Descriptor 0 ------
bLength                  : 0x04 (4 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language ID[0]           : 0x0409 (English - United States)
Data (HexDump)           : 04 03 09 04                                       ....
             ------ String Descriptor 2 ------
bLength                  : 0x22 (34 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Driving Force GT"
Data (HexDump)           : 22 03 44 00 72 00 69 00 76 00 69 00 6E 00 67 00   ".D.r.i.v.i.n.g.
                           20 00 46 00 6F 00 72 00 63 00 65 00 20 00 47 00    .F.o.r.c.e. .G.
                           54 00                                             T.
```