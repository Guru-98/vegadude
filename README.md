# vegadude

vegadude is a utility application uploading programs on CDAC's VEGA Microprocessors.

It is heavily under development and currently only uploading via Serial + XMODEM+CRC-16 has been implemented.


## Clone

```
git clone https://github.com/rnayabed/vegadude.git
```

## Build

```
cmake -B build -S vegadude -DCMAKE_BUILD_TYPE=Release
cmake --build build
```

## Run

```
./build/vegadude -tp /dev/ttyUSB0 -bp <path to binary> -ssb 1 -sbi 8 -sba 115200 -sau
```

## Note

vegadude does not play well with sniffer programs like `interceptty`, *for now*.