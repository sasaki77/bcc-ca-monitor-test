# BCC EPICS Channel Access Monitor

This is the test codes for BCC to monitor the packets of EPICS Channel Access.

The codes is derived from [BCC example codes](https://github.com/iovisor/bcc/tree/master/examples/networking/http_filter).

## Requirements

- BCC: Refer to the [install manual](https://github.com/iovisor/bcc/blob/master/INSTALL.md)

## Usage

```
$ sudo python3 caput-monitor.py -i <interface name>
binding socket to '<interface name>'
load eBPF program
start
Write: ET_SASAKI:TEST2 28 from XXX.XXX.XXX.XXX:pppp to YYY.YYY.YYY.YYY:qqqq
Write: ET_SASAKI:TEST2 28 from XXX.XXX.XXX.XXX:pppp to YYY.YYY.YYY.YYY:qqqq
Write: ET_SASAKI:TEST1 1 from XXX.XXX.XXX.XXX:pppp to YYY.YYY.YYY.YYY:qqqq
Write: ET_SASAKI:TEST1 2 from XXX.XXX.XXX.XXX:pppp to YYY.YYY.YYY.YYY:qqqq
```
