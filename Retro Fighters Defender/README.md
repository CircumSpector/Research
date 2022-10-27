# Retro Fighters Defender

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
