# spidump - Linux SPI dump (tracer)
spidump dumps SPI transfers initiated by linux kernel drivers or userspace by using tracepoint. 

## Requirements
- linux with BPF tracepoints and BTF enabled
- latest bpftrace from git

## Usage
```sh
$ ./spidump
39258003093879 spi0.0 len   14
  TX 90 2c 40 00 00 00 00 00 00 00 00 00 00 00
  RX 00 24 60 47 aa 04 de ad be ef 32 4e a0 e5
39258003124195 spi0.0 len    4
  TX 03 2c 40 00
  RX 00 00 00 00
...
```

