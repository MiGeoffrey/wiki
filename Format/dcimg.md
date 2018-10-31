# dcimg

The `.dcimg` is the output format of the HCI-Image Hammamastu camera software.
It is a binary image with the following structure:

- a header
- blocks
  - timestamp
  - clock

The different versions of the software have different size for this fields :

## v 4.4.0.11

```toml
header = 1206 # bytes
clockskip = 32 # bytes
```

## v*

```toml
header = 808 # bytes
clockskip = 16 # bytes
```





