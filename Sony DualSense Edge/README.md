# Sony DualSense Edge

## UsbTreeView

```text

    =========================== USB Port3 ===========================

Connection Status        : 0x01 (Device is connected)
Port Chain               : 5-3
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
Device Description       : USB Composite Device
Device Path              : \\?\usb#vid_054c&pid_0df2#8&1265ce96&0&3#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device ID                : USB\VID_054C&PID_0DF2\8&1265CE96&0&3
Hardware IDs             : USB\VID_054C&PID_0DF2&REV_0100 USB\VID_054C&PID_0DF2
Driver KeyName           : {36fc9e60-c465-11cf-8056-444553540000}\0046 (GUID_DEVCLASS_USB)
Driver                   : \SystemRoot\System32\drivers\usbccgp.sys (Version: 10.0.19041.1949  Date: 2022-09-16)
Driver Inf               : C:\WINDOWS\inf\usb.inf
Legacy BusType           : PNPBus
Class                    : USB
Class GUID               : {36fc9e60-c465-11cf-8056-444553540000} (GUID_DEVCLASS_USB)
Interface GUID           : {a5dcbf10-6530-11d2-901f-00c04fb951ed} (GUID_DEVINTERFACE_USB_DEVICE)
Service                  : usbccgp
Enumerator               : USB
Location Info            : Port_#0003.Hub_#0002
Location IDs             : PCIROOT(0)#PCI(0102)#PCI(0000)#PCI(0800)#PCI(0003)#USBROOT(0)#USB(3), ACPI(_SB_)#ACPI(PCI0)#ACPI(BXBR)#ACPI(BYUP)#ACPI(BYD8)#ACPI(XHC0)#ACPI(RHUB)#ACPI(PRT3)
Container ID             : {d5b6ed0b-a492-11ed-9473-886dae3ccb7f}
Manufacturer Info        : (Standard USB Host Controller)
Capabilities             : 0x84 (Removable, SurpriseRemovalOK)
Status                   : 0x0180600A (DN_DRIVER_LOADED, DN_STARTED, DN_DISABLEABLE, DN_REMOVABLE, DN_NT_ENUMERATOR, DN_NT_DRIVER)
Problem Code             : 0
Address                  : 3
Power State              : D0 (supported: D0, D3, wake from D0)
 Child Device 1          : DualSense Edge Wireless Controller (USB Audio Device)
  DevicePath             : \\?\usb#vid_054c&pid_0df2&mi_00#9&2816ce0&0&0000#{6994ad04-93ef-11d0-a3cc-00a0c9223196}
  KernelName             : \Device\0000013a
  Device ID              : USB\VID_054C&PID_0DF2&MI_00\9&2816CE0&0&0000
  Class                  : MEDIA
   Child Device 1        : Speakers (DualSense Edge Wireless Controller) (Audio Endpoint)
    DevicePath           : \\?\swd#mmdevapi#{0.0.0.00000000}.{15144b3d-809f-487d-938b-9406c6ff2fa4}#{e6327cad-dcec-4949-ae8a-991e976a79d2}
    KernelName           : \Device\0000013f
    Device ID            : SWD\MMDEVAPI\{0.0.0.00000000}.{15144B3D-809F-487D-938B-9406C6FF2FA4}
    Class                : AudioEndpoint
   Child Device 2        : Headset Microphone (DualSense Edge Wireless Controller) (Audio Endpoint)
    DevicePath           : \\?\swd#mmdevapi#{0.0.1.00000000}.{8f900ea9-a61c-42c4-8512-3bb91d0adc0f}#{2eef81be-33fa-4800-9670-1cd474972c3f}
    KernelName           : \Device\0000013e
    Device ID            : SWD\MMDEVAPI\{0.0.1.00000000}.{8F900EA9-A61C-42C4-8512-3BB91D0ADC0F}
    Class                : AudioEndpoint
 Child Device 2          : USB Input Device
  DevicePath             : \\?\usb#vid_054c&pid_0df2&mi_03#9&2816ce0&0&0003#{86431f5b-9f5a-48ce-8fbf-a537413ef358}
  KernelName             : \Device\0000013b
  Device ID              : USB\VID_054C&PID_0DF2&MI_03\9&2816CE0&0&0003
  Class                  : HIDClass
   Child Device 1        : HID-compliant game controller
    DevicePath           : \\?\hid#vid_054c&pid_0df2&mi_03#a&2aa63a75&0&0000#{4d1e55b2-f16f-11cf-88cb-001111000030}
    KernelName           : \Device\0000013d
    Device ID            : HID\VID_054C&PID_0DF2&MI_03\A&2AA63A75&0&0000
    Class                : HIDClass

        +++++++++++++++++ Registry USB Flags +++++++++++++++++
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\usbflags\054C0DF20100
 osvc                    : REG_BINARY 00 00

        ---------------- Connection Information ---------------
Connection Index         : 0x03 (3)
Connection Status        : 0x01 (DeviceConnected)
Current Config Value     : 0x01
Device Address           : 0x03 (3)
Is Hub                   : 0x00 (no)
Device Bus Speed         : 0x02 (High-Speed)
Number Of Open Pipes     : 0x02 (2 pipes to data endpoints)
Pipe[0]                  : EndpointID=4  Direction=IN   ScheduleOffset=0  Type=Interrupt
Pipe[1]                  : EndpointID=3  Direction=OUT  ScheduleOffset=0  Type=Interrupt
Data (HexDump)           : 03 00 00 00 12 01 00 02 00 00 00 40 4C 05 F2 0D   ...........@L...
                           00 01 01 02 00 01 01 02 00 03 00 02 00 00 00 01   ................
                           00 00 00 07 05 84 03 40 00 04 00 00 00 00 07 05   .......@........
                           03 03 40 00 06 00 00 00 00                        ..@......

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
idProduct                : 0x0DF2
bcdDevice                : 0x0100
iManufacturer            : 0x01 (String Descriptor 1)
 Language 0x0409         : "Sony Interactive Entertainment"
iProduct                 : 0x02 (String Descriptor 2)
 Language 0x0409         : "DualSense Edge Wireless Controller"
iSerialNumber            : 0x00 (No String Descriptor)
bNumConfigurations       : 0x01 (1 Configuration)
Data (HexDump)           : 12 01 00 02 00 00 00 40 4C 05 F2 0D 00 01 01 02   .......@L.......
                           00 01                                             ..

    ------------------ Configuration Descriptor -------------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x02 (Configuration Descriptor)
wTotalLength             : 0x00E3 (227 bytes)
bNumInterfaces           : 0x04 (4 Interfaces)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xC0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x01 (yes)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 02 E3 00 04 01 00 C0 FA 09 04 00 00 00 01 01   ................
                           00 00 0A 24 01 00 01 49 00 02 01 02 0C 24 02 01   ...$...I.....$..
                           01 01 06 04 33 00 00 00 0C 24 06 02 01 01 03 00   ....3....$......
                           00 00 00 00 09 24 03 03 01 03 04 02 00 0C 24 02   .....$........$.
                           04 02 04 03 02 03 00 00 00 09 24 06 05 04 01 03   ..........$.....
                           00 00 09 24 03 06 01 01 01 05 00 09 04 01 00 00   ...$............
                           01 02 00 00 09 04 01 01 01 01 02 00 00 07 24 01   ..............$.
                           01 01 01 00 0B 24 02 01 04 02 10 01 80 BB 00 09   .....$..........
                           05 01 09 88 01 04 00 00 07 25 01 00 00 00 00 09   .........%......
                           04 02 00 00 01 02 00 00 09 04 02 01 01 01 02 00   ................
                           00 07 24 01 06 01 01 00 0B 24 02 01 02 02 10 01   ..$......$......
                           80 BB 00 09 05 82 05 C4 00 04 00 00 07 25 01 00   .............%..
                           00 00 00 09 04 03 00 02 03 00 00 00 09 21 11 01   .............!..
                           00 01 22 85 01 07 05 84 03 40 00 04 07 05 03 03   .."......@......
                           40 00 06                                          @..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
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
wTotalLength             : 0x0049 (73 bytes)
bInCollection            : 0x02
baInterfaceNr[1]         : 0x01
baInterfaceNr[2]         : 0x02
Data (HexDump)           : 0A 24 01 00 01 49 00 02 01 02                     .$...I....

        ------- Audio Control Input Terminal Descriptor -------
bLength                  : 0x0C (12 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Input Terminal)
bTerminalID              : 0x01
wTerminalType            : 0x0101 (USB streaming)
bAssocTerminal           : 0x06
bNrChannels              : 0x04 (4 channels)
wChannelConfig           : 0x0033 (L, R, LS, RS)
iChannelNames            : 0x00 (No String Descriptor)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 02 01 01 01 06 04 33 00 00 00               .$......3...

        -------- Audio Control Feature Unit Descriptor --------
bLength                  : 0x0C (12 bytes)
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
bmaControls[3]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
bmaControls[4]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
iFeature                 : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 06 02 01 01 03 00 00 00 00 00               .$..........

        ------- Audio Control Output Terminal Descriptor ------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x03 (Output Terminal)
bTerminalID              : 0x03
wTerminalType            : 0x0301 (Speaker)
bAssocTerminal           : 0x04 (4)
bSourceID                : 0x02 (2)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 03 03 01 03 04 02 00                        .$.......

        ------- Audio Control Input Terminal Descriptor -------
bLength                  : 0x0C (12 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Input Terminal)
bTerminalID              : 0x04
wTerminalType            : 0x0402 (Headset)
bAssocTerminal           : 0x03
bNrChannels              : 0x02 (2 channels)
wChannelConfig           : 0x0003 (L, R)
iChannelNames            : 0x00 (No String Descriptor)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 02 04 02 04 03 02 03 00 00 00               .$..........

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
wTerminalType            : 0x0101 (USB streaming)
bAssocTerminal           : 0x01 (1)
bSourceID                : 0x05 (5)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 03 06 01 01 01 05 00                        .$.......

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x01
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
bInterfaceNumber         : 0x01
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
bDescriptorSubtype       : 0x01
bTerminalLink            : 0x01
bDelay                   : 0x01
wFormatTag               : 0x0001 (PCM)
Data (HexDump)           : 07 24 01 01 01 01 00                              .$.....

        ------- Audio Streaming Format Type Descriptor --------
bLength                  : 0x0B (11 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Format Type)
bFormatType              : 0x01 (FORMAT_TYPE_I)
bNrChannels              : 0x04 (4 channels)
bSubframeSize            : 0x02 (2 bytes per subframe)
bBitResolution           : 0x10 (16 bits per sample)
bSamFreqType             : 0x01 (supports 1 sample frequence)
tSamFreq[1]              : 0x0BB80 (48000 Hz)
Data (HexDump)           : 0B 24 02 01 04 02 10 01 80 BB 00                  .$.........

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x01 (Direction=OUT EndpointID=1)
bmAttributes             : 0x09 (TransferType=Isochronous  SyncType=Adaptive  EndpointType=Data)
wMaxPacketSize           : 0x0188
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0x188 (392 bytes per packet)
bInterval                : 0x04 (4 ms)
bRefresh                 : 0x00
bSynchAddress            : 0x00
Data (HexDump)           : 09 05 01 09 88 01 04 00 00                        .........

        ----------- Audio Data Endpoint Descriptor ------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x25 (Audio Endpoint Descriptor)
bDescriptorSubtype       : 0x01 (General)
bmAttributes             : 0x00
bLockDelayUnits          : 0x00
wLockDelay               : 0x0000
Data (HexDump)           : 07 25 01 00 00 00 00                              .%.....

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x02
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
bInterfaceNumber         : 0x02
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
bDescriptorSubtype       : 0x01
bTerminalLink            : 0x06
bDelay                   : 0x01
wFormatTag               : 0x0001 (PCM)
Data (HexDump)           : 07 24 01 06 01 01 00                              .$.....

        ------- Audio Streaming Format Type Descriptor --------
bLength                  : 0x0B (11 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Format Type)
bFormatType              : 0x01 (FORMAT_TYPE_I)
bNrChannels              : 0x02 (2 channels)
bSubframeSize            : 0x02 (2 bytes per subframe)
bBitResolution           : 0x10 (16 bits per sample)
bSamFreqType             : 0x01 (supports 1 sample frequence)
tSamFreq[1]              : 0x0BB80 (48000 Hz)
Data (HexDump)           : 0B 24 02 01 02 02 10 01 80 BB 00                  .$.........

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x82 (Direction=IN EndpointID=2)
bmAttributes             : 0x05 (TransferType=Isochronous  SyncType=Asynchronous  EndpointType=Data)
wMaxPacketSize           : 0x00C4
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0xC4 (196 bytes per packet)
bInterval                : 0x04 (4 ms)
bRefresh                 : 0x00
bSynchAddress            : 0x00
Data (HexDump)           : 09 05 82 05 C4 00 04 00 00                        .........

        ----------- Audio Data Endpoint Descriptor ------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x25 (Audio Endpoint Descriptor)
bDescriptorSubtype       : 0x01 (General)
bmAttributes             : 0x00
bLockDelayUnits          : 0x00
wLockDelay               : 0x0000
Data (HexDump)           : 07 25 01 00 00 00 00                              .%.....

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x03
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
Data (HexDump)           : 09 21 11 01 00 01 22 85 01                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0185 (389 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x84 (Direction=IN EndpointID=4)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0x40 (64 bytes per packet)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 84 03 40 00 04                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x03 (Direction=OUT EndpointID=3)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0x40 (64 bytes per packet)
bInterval                : 0x06 (6 ms)
Data (HexDump)           : 07 05 03 03 40 00 06                              ....@..

    ----------------- Device Qualifier Descriptor -----------------
bLength                  : 0x0A (10 bytes)
bDescriptorType          : 0x06 (Device_qualifier Descriptor)
bcdUSB                   : 0x200 (USB Version 2.00)
bDeviceClass             : 0x00 (defined by the interface descriptors)
bDeviceSubClass          : 0x00
bDeviceProtocol          : 0x00
bMaxPacketSize0          : 0x40 (64 Bytes)
bNumConfigurations       : 0x01 (1 other-speed configuration)
bReserved                : 0x00

    ------------ Other Speed Configuration Descriptor -------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x07 (Other_speed_configuration Descriptor)
wTotalLength             : 0x00E3 (227 bytes)
bNumInterfaces           : 0x04 (4 Interfaces)
bConfigurationValue      : 0x01 (Configuration 1)
iConfiguration           : 0x00 (No String Descriptor)
bmAttributes             : 0xC0
 D7: Reserved, set 1     : 0x01
 D6: Self Powered        : 0x01 (yes)
 D5: Remote Wakeup       : 0x00 (no)
 D4..0: Reserved, set 0  : 0x00
MaxPower                 : 0xFA (500 mA)
Data (HexDump)           : 09 07 E3 00 04 01 00 C0 FA 09 04 00 00 00 01 01   ................
                           00 00 0A 24 01 00 01 49 00 02 01 02 0C 24 02 01   ...$...I.....$..
                           01 01 06 04 33 00 00 00 0C 24 06 02 01 01 03 00   ....3....$......
                           00 00 00 00 09 24 03 03 01 03 04 02 00 0C 24 02   .....$........$.
                           04 02 04 03 01 00 00 00 00 09 24 06 05 04 01 03   ..........$.....
                           00 00 09 24 03 06 01 01 01 05 00 09 04 01 00 00   ...$............
                           01 02 00 00 09 04 01 01 01 01 02 00 00 07 24 01   ..............$.
                           01 01 01 00 0B 24 02 01 04 02 10 01 80 BB 00 09   .....$..........
                           05 01 09 88 01 01 00 00 07 25 01 01 00 00 00 09   .........%......
                           04 02 00 00 01 02 00 00 09 04 02 01 01 01 02 00   ................
                           00 07 24 01 06 01 01 00 0B 24 02 01 02 02 10 01   ..$......$......
                           80 BB 00 09 05 82 05 C4 00 01 00 00 07 25 01 00   .............%..
                           00 00 00 09 04 03 00 02 03 00 00 00 09 21 11 01   .............!..
                           00 01 22 85 01 07 05 84 03 40 00 04 07 05 03 03   .."......@......
                           40 00 06                                          @..

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x00
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
wTotalLength             : 0x0049 (73 bytes)
bInCollection            : 0x02
baInterfaceNr[1]         : 0x01
baInterfaceNr[2]         : 0x02
Data (HexDump)           : 0A 24 01 00 01 49 00 02 01 02                     .$...I....

        ------- Audio Control Input Terminal Descriptor -------
bLength                  : 0x0C (12 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Input Terminal)
bTerminalID              : 0x01
wTerminalType            : 0x0101 (USB streaming)
bAssocTerminal           : 0x06
bNrChannels              : 0x04 (4 channels)
wChannelConfig           : 0x0033 (L, R, LS, RS)
iChannelNames            : 0x00 (No String Descriptor)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 02 01 01 01 06 04 33 00 00 00               .$......3...

        -------- Audio Control Feature Unit Descriptor --------
bLength                  : 0x0C (12 bytes)
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
bmaControls[3]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
bmaControls[4]           : 0x00
 D0: Mute                : 0
 D1: Volume              : 0
 D2: Bass                : 0
 D3: Mid                 : 0
 D4: Treble              : 0
 D5: Graphic Equalizer   : 0
 D6: Automatic Gain      : 0
 D7: Delay               : 0
iFeature                 : 0x00 (No String Descriptor)
Data (HexDump)           : 0C 24 06 02 01 01 03 00 00 00 00 00               .$..........

        ------- Audio Control Output Terminal Descriptor ------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x03 (Output Terminal)
bTerminalID              : 0x03
wTerminalType            : 0x0301 (Speaker)
bAssocTerminal           : 0x04 (4)
bSourceID                : 0x02 (2)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 03 03 01 03 04 02 00                        .$.......

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
wTerminalType            : 0x0101 (USB streaming)
bAssocTerminal           : 0x01 (1)
bSourceID                : 0x05 (5)
iTerminal                : 0x00 (No String Descriptor)
Data (HexDump)           : 09 24 03 06 01 01 01 05 00                        .$.......

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x01
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
bInterfaceNumber         : 0x01
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
bDescriptorSubtype       : 0x01
bTerminalLink            : 0x01
bDelay                   : 0x01
wFormatTag               : 0x0001 (PCM)
Data (HexDump)           : 07 24 01 01 01 01 00                              .$.....

        ------- Audio Streaming Format Type Descriptor --------
bLength                  : 0x0B (11 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Format Type)
bFormatType              : 0x01 (FORMAT_TYPE_I)
bNrChannels              : 0x04 (4 channels)
bSubframeSize            : 0x02 (2 bytes per subframe)
bBitResolution           : 0x10 (16 bits per sample)
bSamFreqType             : 0x01 (supports 1 sample frequence)
tSamFreq[1]              : 0x0BB80 (48000 Hz)
Data (HexDump)           : 0B 24 02 01 04 02 10 01 80 BB 00                  .$.........

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x01 (Direction=OUT EndpointID=1)
bmAttributes             : 0x09 (TransferType=Isochronous  SyncType=Adaptive  EndpointType=Data)
wMaxPacketSize           : 0x0188
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0x188 (392 bytes per packet)
bInterval                : 0x01 (1 ms)
bRefresh                 : 0x00
bSynchAddress            : 0x00
Data (HexDump)           : 09 05 01 09 88 01 01 00 00                        .........

        ----------- Audio Data Endpoint Descriptor ------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x25 (Audio Endpoint Descriptor)
bDescriptorSubtype       : 0x01 (General)
bmAttributes             : 0x01
bLockDelayUnits          : 0x00
wLockDelay               : 0x0000
Data (HexDump)           : 07 25 01 01 00 00 00                              .%.....

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x02
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
bInterfaceNumber         : 0x02
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
bDescriptorSubtype       : 0x01
bTerminalLink            : 0x06
bDelay                   : 0x01
wFormatTag               : 0x0001 (PCM)
Data (HexDump)           : 07 24 01 06 01 01 00                              .$.....

        ------- Audio Streaming Format Type Descriptor --------
bLength                  : 0x0B (11 bytes)
bDescriptorType          : 0x24 (Audio Interface Descriptor)
bDescriptorSubtype       : 0x02 (Format Type)
bFormatType              : 0x01 (FORMAT_TYPE_I)
bNrChannels              : 0x02 (2 channels)
bSubframeSize            : 0x02 (2 bytes per subframe)
bBitResolution           : 0x10 (16 bits per sample)
bSamFreqType             : 0x01 (supports 1 sample frequence)
tSamFreq[1]              : 0x0BB80 (48000 Hz)
Data (HexDump)           : 0B 24 02 01 02 02 10 01 80 BB 00                  .$.........

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x82 (Direction=IN EndpointID=2)
bmAttributes             : 0x05 (TransferType=Isochronous  SyncType=Asynchronous  EndpointType=Data)
wMaxPacketSize           : 0x00C4
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0xC4 (196 bytes per packet)
bInterval                : 0x01 (1 ms)
bRefresh                 : 0x00
bSynchAddress            : 0x00
Data (HexDump)           : 09 05 82 05 C4 00 01 00 00                        .........

        ----------- Audio Data Endpoint Descriptor ------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x25 (Audio Endpoint Descriptor)
bDescriptorSubtype       : 0x01 (General)
bmAttributes             : 0x00
bLockDelayUnits          : 0x00
wLockDelay               : 0x0000
Data (HexDump)           : 07 25 01 00 00 00 00                              .%.....

        ---------------- Interface Descriptor -----------------
bLength                  : 0x09 (9 bytes)
bDescriptorType          : 0x04 (Interface Descriptor)
bInterfaceNumber         : 0x03
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
Data (HexDump)           : 09 21 11 01 00 01 22 85 01                        .!...."..
Descriptor 1:
bDescriptorType          : 0x22 (Class=Report)
wDescriptorLength        : 0x0185 (389 bytes)
Error reading descriptor : ERROR_INVALID_PARAMETER

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x84 (Direction=IN EndpointID=4)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0x40 (64 bytes per packet)
bInterval                : 0x04 (4 ms)
Data (HexDump)           : 07 05 84 03 40 00 04                              ....@..

        ----------------- Endpoint Descriptor -----------------
bLength                  : 0x07 (7 bytes)
bDescriptorType          : 0x05 (Endpoint Descriptor)
bEndpointAddress         : 0x03 (Direction=OUT EndpointID=3)
bmAttributes             : 0x03 (TransferType=Interrupt)
wMaxPacketSize           : 0x0040
 Bits 15..13             : 0x00 (reserved, must be zero)
 Bits 12..11             : 0x00 (0 additional transactions per microframe -> allows 1..1024 bytes per packet)
 Bits 10..0              : 0x40 (64 bytes per packet)
bInterval                : 0x06 (6 ms)
Data (HexDump)           : 07 05 03 03 40 00 06                              ....@..

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
bLength                  : 0x46 (70 bytes)
bDescriptorType          : 0x03 (String Descriptor)
Language 0x0409          : "DualSense Edge Wireless Controller"
Data (HexDump)           : 46 03 44 00 75 00 61 00 6C 00 53 00 65 00 6E 00   F.D.u.a.l.S.e.n.
                           73 00 65 00 20 00 45 00 64 00 67 00 65 00 20 00   s.e. .E.d.g.e. .
                           57 00 69 00 72 00 65 00 6C 00 65 00 73 00 73 00   W.i.r.e.l.e.s.s.
                           20 00 43 00 6F 00 6E 00 74 00 72 00 6F 00 6C 00    .C.o.n.t.r.o.l.
                           6C 00 65 00 72 00                                 l.e.r.

```
