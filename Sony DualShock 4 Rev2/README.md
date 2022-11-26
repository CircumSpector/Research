# Sony DualShock 4 Rev2

## UsbTreeView

```text

    =========================== USB Port12 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 1-12

      ========================== Summary =========================
Vendor ID                : 0x054C (Sony Group Corporation)
Product ID               : 0x09CC
USB Version              : 2.0 -> but Device is Full-Speed only
Port maximum Speed       : High-Speed
Device maximum Speed     : Full-Speed
Device Connection Speed  : Full-Speed
Self powered             : yes
Demanded Current         : 500 mA
Used Endpoints           : 3

      ======================== USB Device ========================

        +++++++++++++++++ Device Information ++++++++++++++++++
Device Description       : USB Composite Device
Device Path              : \\?\USB#VID_054C&PID_09CC#6&3af0f9ce&0&12#{a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Kernel Name              : \Device\USBPDO-6
Device ID                : USB\VID_054C&PID_09CC\6&3AF0F9CE&0&12
Hardware IDs             : USB\VID_054C&PID_09CC&REV_0100 USB\VID_054C&PID_09CC
Driver KeyName           : {36fc9e60-c465-11cf-8056-444553540000}\0007 (GUID_DEVCLASS_USB)
Driver                   : \SystemRoot\System32\drivers\usbccgp.sys (Version: 10.0.22621.608  Date: 2022-10-11)
Driver Inf               : C:\Windows\inf\usb.inf
Legacy BusType           : PNPBus
Class                    : USB
Class GUID               : {36fc9e60-c465-11cf-8056-444553540000} (GUID_DEVCLASS_USB)
Service                  : usbccgp
Enumerator               : USB
Location Info            : Port_#0012.Hub_#0001
Location IDs             : PCIROOT(0)#PCI(0103)#PCI(0000)#USBROOT(0)#USB(12), ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP2)#ACPI(PTXH)#ACPI(RHUB)#ACPI(PO12)
Container ID             : {050425c3-6792-11ed-9655-eb0b22d79654}
Manufacturer Info        : (Standard USB Host Controller)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Address                  : 12
HcDisableSelectiveSuspend: 0
EnableSelectiveSuspend   : 0
SelectiveSuspendEnabled  : 0
EnhancedPowerMgmtEnabled : 0
IdleInWorkingState       : 0
WakeFromSleepState       : 0
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : Wireless Controller (USB Audio Device)
  Device Path 1          : \\?\USB#VID_054C&PID_09CC&MI_00#7&1f92565f&1&0000#{6994ad04-93ef-11d0-a3cc-00a0c9223196}\global (AM_KSCATEGORY_AUDIO)
  Device Path 2          : \\?\USB#VID_054C&PID_09CC&MI_00#7&1f92565f&1&0000#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\global (AM_KSCATEGORY_CAPTURE)
  Device Path 3          : \\?\USB#VID_054C&PID_09CC&MI_00#7&1f92565f&1&0000#{65e8773e-8f56-11d0-a3b9-00a0c9223196}\global (AM_KSCATEGORY_RENDER)
  Kernel Name            : \Device\0000008e
  Device ID              : USB\VID_054C&PID_09CC&MI_00\7&1F92565F&1&0000
  Class                  : MEDIA
  Driver KeyName         : {4d36e96c-e325-11ce-bfc1-08002be10318}\0009 (GUID_DEVCLASS_MEDIA)
  Service                : usbaudio
  Location               : 0001.0000.0000.012.000.000.000.000.000
  LocationPaths          : PCIROOT(0)#PCI(0103)#PCI(0000)#USBROOT(0)#USB(12)#USBMI(0)  PCIROOT(0)#PCI(0103)#PCI(0000)#USBROOT(0)#USB(12)#USB(12)  ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP2)#ACPI(PTXH)#ACPI(RHUB)#ACPI(PO12)#USBMI(0)  ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP2)#ACPI(PTXH)#ACPI(RHUB)#ACPI(PO12)#USB(12)
   Child Device 1        : Headset Earphone (Wireless Controller) (Audio Endpoint)
    Device ID            : SWD\MMDEVAPI\{0.0.0.00000000}.{0063026E-DE72-44D0-B1D8-336A73A8293E}
    Class                : AudioEndpoint
    Driver KeyName       : {c166523c-fe0c-4a94-a586-f1a80cfbbf3e}\0007 (AUDIOENDPOINT_CLASS_UUID)
   Child Device 2        : Headset Microphone (Wireless Controller) (Audio Endpoint)
    Device ID            : SWD\MMDEVAPI\{0.0.1.00000000}.{0D146A01-EC06-4B5F-99EA-5B396A9B4020}
    Class                : AudioEndpoint
    Driver KeyName       : {c166523c-fe0c-4a94-a586-f1a80cfbbf3e}\0006 (AUDIOENDPOINT_CLASS_UUID)
 Child Device 2          : USB Input Device
  Device ID              : USB\VID_054C&PID_09CC&MI_03\7&1F92565F&1&0003
  Class                  : HIDClass
  Driver KeyName         : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0020 (GUID_DEVCLASS_HIDCLASS)
  Service                : HidUsb
  Location               : 0001.0000.0000.012.000.000.000.000.000
  LocationPaths          : PCIROOT(0)#PCI(0103)#PCI(0000)#USBROOT(0)#USB(12)#USBMI(3)  ACPI(_SB_)#ACPI(PCI0)#ACPI(GPP2)#ACPI(PTXH)#ACPI(RHUB)#ACPI(PO12)#USBMI(3)
   Child Device 1        : HID-compliant game controller
    Device Path          : \\?\HID#VID_054C&PID_09CC&MI_03#8&365433fc&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030} (GUID_DEVINTERFACE_HID)
    Kernel Name          : \Device\00000091
    Device ID            : HID\VID_054C&PID_09CC&MI_03\8&365433FC&0&0000
    Class                : HIDClass
    Driver KeyName       : {745a17a0-74d3-11d0-b6fe-00a0c90f57da}\0021 (GUID_DEVCLASS_HIDCLASS)

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\054C09CC0100
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x0C (Port 12)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01 (Configuration 1)
Device Address           : 0x04 (4)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x01 (Full-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=4  Direction=IN   ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x40    bInterval=5   -> 718 Bits/ms = 89750 Bytes/s
Pipe[1]                  : EndpointID=3  Direction=OUT  ScheduleOffset=0  Type=Interrupt  wMaxPacketSize=0x40    bInterval=5   -> 718 Bits/ms = 89750 Bytes/s
Data (HexDump)           : 0C 00 00 00 12 01 00 02 00 00 00 40 4C 05 CC 09   ...........@L...
                           00 01 01 02 00 01 01 01 00 04 00 02 00 00 00 01   ................
                           00 00 00 07 05 84 03 40 00 05 00 00 00 00 07 05   .......@........
                           03 03 40 00 05 00 00 00 00                        ..@......

        --------------- Connection Information V2 -------------
Connection Index         : 0x0C (12)
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
Data (HexDump)           : 0C 00 00 00 10 00 00 00 03 00 00 00 00 00 00 00   ................

    ---------------------- Device Descriptor ----------------------
bLength                  : 0x12 (18 bytes)
bDescriptorType          : 0x01 (Device Descriptor)
bcdUSB                   : 0x200 (USB Version 2.0) -> but device is Full-Speed only
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 bytes)
idVendor                 : 0x054C (Sony Group Corporation)
idProduct                : 0x09CC
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Sony Interactive Entertainment"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "Wireless Controller"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 40 4C 05 CC 09 00 01 01 02   .......@L.......
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x00E1 (225 bytes)
bNumInterfaces           : 0x04 (4 Interfaces)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xC0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x01 (yes)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 02 E1 00 04 01 00 C0 FA 09 04 00 00 00 01 01   ................
                           00 00 0A 24 01 00 01 47 00 02 01 02 0C 24 02 01   ...$...G.....$..
                           01 01 06 02 03 00 00 00 0A 24 06 02 01 01 03 00   .........$......
                           00 00 09 24 03 03 02 04 04 02 00 0C 24 02 04 02   ...$........$...
                           04 03 01 00 00 00 00 09 24 06 05 04 01 03 00 00   ........$.......
                           09 24 03 06 01 01 01 05 00 09 04 01 00 00 01 02   .$..............
                           00 00 09 04 01 01 01 01 02 00 00 07 24 01 01 01   ............$...
                           01 00 0B 24 02 01 02 02 10 01 00 7D 00 09 05 01   ...$.......}....
                           09 84 00 01 00 00 07 25 01 00 00 00 00 09 04 02   .......%........
                           00 00 01 02 00 00 09 04 02 01 01 01 02 00 00 07   ................
                           24 01 06 01 01 00 0B 24 02 01 01 02 10 01 80 3E   $......$.......>
                           00 09 05 82 05 22 00 01 00 00 07 25 01 00 00 00   .....".....%....
                           00 09 04 03 00 02 03 00 00 00 09 21 11 01 00 01   ...........!....
                           22 FB 01 07 05 84 03 40 00 05 07 05 03 03 40 00   "......@......@.
                           05                                                .

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00 (Interface 0)
bAlternateSetting        : 0x00
bNumEndpoints            : 0x00 (Default Control Pipe only)
bInterfaceClass          : 0x01 (Audio)
bInterfaceSubClass       : 0x01 (Audio Control)
bInterfaceProtocol       : 0x00
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 00 00 00 01 01 00 00                        .........

        ------ Audio Control Interface Header Descriptor ------
bLength                  : 0x0A (10 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x01 (Header)
bcdADC                   : 0x0100
wTotalLength             : 0x0047 (71 bytes)
bInCollection            : 0x02
baInterfaceNr[1]         : 0x01
baInterfaceNr[2]         : 0x02
Data (HexDump)           : 0A 24 01 00 01 47 00 02 01 02                     .$...G....

        ------- Audio Control Input Terminal Descriptor -------
bLength                  : 0x0C (12 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Input Terminal)
bTerminalID              : 0x01
wTerminalType            : 0x0101 (USB Streaming)
bAssocTerminal           : 0x06
bNrChannels              : 0x02 (2 channels)
wChannelConfig           : 0x0003 (L, R)
iChannelNames            : 0x00 (No String Descriptor)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 02 01 01 01 06 02 03 00 00 00               .$..........

        -------- Audio Control Feature Unit Descriptor --------
bLength                  : 0x0A (10 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x06 (Feature Unit)
bUnitID                  : 0x02 (2)
bSourceID                : 0x01 (1)
bControlSize             : 0x01 (1 byte per control)
bmaControls[0]           : 0x03
 D0: Mute                : 1
 D1: Volume              : 1
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
bmaControls[1]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
bmaControls[2]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
iFeature                 : 0x00 (No String Descriptor)
Data (HexDump)           : 0A 24 06 02 01 01 03 00 00 00                     .$........

        ------- Audio Control Output Terminal Descriptor ------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x03 (Output Terminal)
bTerminalID              : 0x03
wTerminalType            : 0x0402 (Headset)
bAssocTerminal           : 0x04 (4)
bSourceID                : 0x02 (2)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 03 03 02 04 04 02 00                        .$.......

        ------- Audio Control Input Terminal Descriptor -------
bLength                  : 0x0C (12 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Input Terminal)
bTerminalID              : 0x04
wTerminalType            : 0x0402 (Headset)
bAssocTerminal           : 0x03
bNrChannels              : 0x01 (1 channel)
wChannelConfig           : 0x0000 (-)
iChannelNames            : 0x00 (No String Descriptor)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 02 04 02 04 03 01 00 00 00 00               .$..........

        -------- Audio Control Feature Unit Descriptor --------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x06 (Feature Unit)
bUnitID                  : 0x05 (5)
bSourceID                : 0x04 (4)
bControlSize             : 0x01 (1 byte per control)
bmaControls[0]           : 0x03
 D0: Mute                : 1
 D1: Volume              : 1
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
bmaControls[1]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
iFeature                 : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 06 05 04 01 03 00 00                        .$.......

        ------- Audio Control Output Terminal Descriptor ------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x03 (Output Terminal)
bTerminalID              : 0x06
wTerminalType            : 0x0101 (USB Streaming)
bAssocTerminal           : 0x01 (1)
bSourceID                : 0x05 (5)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 03 06 01 01 01 05 00                        .$.......

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x01 (Interface 1)
bAlternateSetting        : 0x00
bNumEndpoints            : 0x00 (Default Control Pipe only)
bInterfaceClass          : 0x01 (Audio)
bInterfaceSubClass       : 0x02 (Audio Streaming)
bInterfaceProtocol       : 0x00
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 01 00 00 01 02 00 00                        .........

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x01 (Interface 1)
bAlternateSetting        : 0x01
bNumEndpoints            : 0x01 (1 Endpoint)
bInterfaceClass          : 0x01 (Audio)
bInterfaceSubClass       : 0x02 (Audio Streaming)
bInterfaceProtocol       : 0x00
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 01 01 01 01 02 00 00                        .........

        -------- Audio Streaming Interface Descriptor ---------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x01 (AS_GENERAL)
bTerminalLink            : 0x01 (Terminal ID 1)
bDelay                   : 0x01 (1 frame)
wFormatTag               : 0x0001 (PCM)
Data (HexDump)           : 07 24 01 01 01 01 00                              .$.....

        ------- Audio Streaming Format Type Descriptor --------
bLength                  : 0x0B (11 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Format Type)
bFormatType              : 0x01 (FORMAT_TYPE_I)
bNrChannels              : 0x02 (2 channels)
bSubframeSize            : 0x02 (2 bytes per subframe)
bBitResolution           : 0x10 (16 bits per sample)
bSamFreqType             : 0x01 (supports 1 sample frequence)
tSamFreq[1]              : 0x07D00 (32000 Hz)
Data (HexDump)           : 0B 24 02 01 02 02 10 01 00 7D 00                  .$.......}.

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x01 (Direction=OUT EndpointID=1)
bmAttributes             : 0x09 (TransferType=Isochronous  SyncType=Adaptive  EndpointType=Data)
wMaxPacketSize           : 0x0084 (132 bytes)
bInterval                : 0x01 (1 ms)
bRefresh                 : 0x00
bSynchAddress            : 0x00
Data (HexDump)           : 09 05 01 09 84 00 01 00 00                        .........

        ----------- Audio Data Endpoint Descriptor ------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x25 (Audio Endpoint Descriptor)
bDescriptorSubtype       : 0x01 (General)
bmAttributes             : 0x00
 D0   : Sampling Freq    : 0x00 (not supported)
 D1   : Pitch            : 0x00 (not supported)
 D6..2: Reserved         : 0x00
 D7   : MaxPacketsOnly   : 0x00 (no)
bLockDelayUnits          : 0x00 (Undefined)
wLockDelay               : 0x0000
Data (HexDump)           : 07 25 01 00 00 00 00                              .%.....

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x02 (Interface 2)
bAlternateSetting        : 0x00
bNumEndpoints            : 0x00 (Default Control Pipe only)
bInterfaceClass          : 0x01 (Audio)
bInterfaceSubClass       : 0x02 (Audio Streaming)
bInterfaceProtocol       : 0x00
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 02 00 00 01 02 00 00                        .........

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x02 (Interface 2)
bAlternateSetting        : 0x01
bNumEndpoints            : 0x01 (1 Endpoint)
bInterfaceClass          : 0x01 (Audio)
bInterfaceSubClass       : 0x02 (Audio Streaming)
bInterfaceProtocol       : 0x00
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 02 01 01 01 02 00 00                        .........

        -------- Audio Streaming Interface Descriptor ---------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x01 (AS_GENERAL)
bTerminalLink            : 0x06 (Terminal ID 6)
bDelay                   : 0x01 (1 frame)
wFormatTag               : 0x0001 (PCM)
Data (HexDump)           : 07 24 01 06 01 01 00                              .$.....

        ------- Audio Streaming Format Type Descriptor --------
bLength                  : 0x0B (11 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Format Type)
bFormatType              : 0x01 (FORMAT_TYPE_I)
bNrChannels              : 0x01 (1 channel)
bSubframeSize            : 0x02 (2 bytes per subframe)
bBitResolution           : 0x10 (16 bits per sample)
bSamFreqType             : 0x01 (supports 1 sample frequence)
tSamFreq[1]              : 0x03E80 (16000 Hz)
Data (HexDump)           : 0B 24 02 01 01 02 10 01 80 3E 00                  .$.......>.

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x82 (Direction=IN EndpointID=2)
bmAttributes             : 0x05 (TransferType=Isochronous  SyncType=Asynchronous  EndpointType=Data)
wMaxPacketSize           : 0x0022 (34 bytes)
bInterval                : 0x01 (1 ms)
bRefresh                 : 0x00
bSynchAddress            : 0x00
Data (HexDump)           : 09 05 82 05 22 00 01 00 00                        ...."....

        ----------- Audio Data Endpoint Descriptor ------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x25 (Audio Endpoint Descriptor)
bDescriptorSubtype       : 0x01 (General)
bmAttributes             : 0x00
 D0   : Sampling Freq    : 0x00 (not supported)
 D1   : Pitch            : 0x00 (not supported)
 D6..2: Reserved         : 0x00
 D7   : MaxPacketsOnly   : 0x00 (no)
bLockDelayUnits          : 0x00 (Undefined)
wLockDelay               : 0x0000
Data (HexDump)           : 07 25 01 00 00 00 00                              .%.....

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x03 (Interface 3)
bAlternateSetting        : 0x00
bNumEndpoints            : 0x02 (2 Endpoints)
bInterfaceClass          : 0x03 (HID - Human Interface Device)
bInterfaceSubClass       : 0x00 (None)
bInterfaceProtocol       : 0x00 (None)
iInterface               : 0x00 (No String Descriptor)
Data (HexDump)           : 09 04 03 00 02 03 00 00 00                        .........

        ------------------- HID Descriptor --------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x21 (HID Descriptor)
bcdHID                   : 0x0111 (HID Version 1.11)
bCountryCode             : 0x00 (00 = not localized)
bNumDescriptors          : 0x01
Data (HexDump)           : 09 21 11 01 00 01 22 FB 01                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x01FB (507 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER (due to a obscure limitation of the Win32 USB API, see UsbTreeView.txt)

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x84 (Direction=IN EndpointID=4)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x05 (5 ms)
Data (HexDump)           : 07 05 84 03 40 00 05                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x03 (Direction=OUT EndpointID=3)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040 (64 bytes)
bInterval                : 0x05 (5 ms)
Data (HexDump)           : 07 05 03 03 40 00 05                              ....@..

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
bLength                  : 0x28 (40 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "Wireless Controller"
Data (HexDump)           : 28 03 57 00 69 00 72 00 65 00 6C 00 65 00 73 00   (.W.i.r.e.l.e.s.
                           73 00 20 00 43 00 6F 00 6E 00 74 00 72 00 6F 00   s. .C.o.n.t.r.o.
                           6C 00 6C 00 65 00 72 00                           l.l.e.r.

```
