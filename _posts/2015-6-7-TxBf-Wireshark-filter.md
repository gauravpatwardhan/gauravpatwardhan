---
layout: post
title: Beamforming Wireshark filters
---

Being a wireless engineer now-a-days I have to filter beamforming packets from wireless traces for debugging purposes so I hope this filter encourages people to play around with beamforming packets.

```
(wlan.fc.type_subtype == 0x15) || (wlan.fc.type_subtype == 0x0e)
```

Please note that this filter will show you packets CORRECTLY decoded only on the wireshark development version 1.99.5 available at https://www.wireshark.org/download.html