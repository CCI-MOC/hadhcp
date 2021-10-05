# HA DHCP Service

This implements a highly available dynamic DHCP service using ISC
DHCPd, mostly following "[A Basic Guide to Configuring DHCP
Failover][kb]".

It also replaces our existing dnsmasq service:

- All static DHCP entries are now served by ISC DHCPd
- Dnsmasq continues to act as a DNS server for the 192.12.185.0/24
  network.

[kb]: https://kb.isc.org/docs/aa-00502
