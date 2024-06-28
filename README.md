# VPN-IPTables
A few VPN iptables that I wrote a while ago that block some commonly seen attacks.

These IPTables block various TCP floods, as well as allow legitimate connections. They also block portscans

There are multiple examples of captured attacks that all have to do with amplification. You can tell that they are amplification because they all have the same source port, and if you open the file in wireshark, all of the requests have unique data but it's for the most part in the same kind of formatting. These attacks are effective in pushing a large amount of data, but can easily be counteracted by dropping any connections that are UDP and with the source port of the vulnerable devices. A picture is shown with the most common ones dropped, and it prioritizes the ones with the most active devices and the highest amplification factor.
