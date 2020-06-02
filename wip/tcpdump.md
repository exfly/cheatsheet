---
title: Tcpdump
category: Hidden
layout: 2017/sheet
tags: [WIP]
intro: |
  `tcpdump` libcapt network data
---

### Tcpdump

```bash
sudo tcpdump -i captain0 -s 1600 -w capture.pcap
sudo tcpreplay -i captain0 --pktlen capture.pcap
tshark -r capture.pcap

sudo ip link add name captain0 type bridge
sudo ip link set captain0 up
```

## References
