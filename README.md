# iperf notes

Great tool for troubleshooting and testing network connectivity between hosts.

### Installation

* CentOS: yum install iperf3 -y
* Ubuntu: apt install iperf3 -y

### Server side usage

* TCP: iperf3 -s
* UDP: iperf3 -s -u

### Client side usage and outputs

``iperf3 -c [ip] -t [time] -i [interval] -f [unit]``

``iperf3 -c 144.202.93.99 -t 600 -i 1 -f m -R ``

```
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bandwidth       Retr
[  4]   0.00-30.00  sec  18.3 GBytes  5234 Mbits/sec   35             sender
[  4]   0.00-30.00  sec  18.3 GBytes  5233 Mbits/sec                  receiver
```


