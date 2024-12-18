# Sony DualShock 3

## Captures

The `.pcap` files can be inspected with Wireshark. Use the following filter to hide the less interesting packet types:

```text
(((!(usbll.pid == 0xd2)) && !(usbll.pid == 0xa5)) && !(usbll.pid == 0x5a)) && !(usbll.pid == 0x69)
```

### Find host address requests

```text
usb.setup.wValue == 0x03F5
```

### Find outgoing requests

```text
(usbll.reassembled.length >= 49) && (usbll.src == "host")
```

### Rumble capture test method

Regarding file `2024-05-13_DS3-CECHZC2E-A1_PS3_Rumble_Tests.pcap`:

- 3 times small motor rumble
- 3 times big motor rumble
- 3 times both motors rumble

## Models/Revisions

### CECHZC2E-A1

- Doesn't support being turned off on USB (console doesn't offer "Turn off controller" when holding PS)

### CECHZC2E-B1

### CECHZC2U-A2

### SIXAXIS (no model no.)
