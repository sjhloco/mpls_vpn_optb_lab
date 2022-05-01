# MPLS-VPN OptionB Lab

The configuration files from a blog post I wrote about [MPLS-VPN OptionB (Inter-AS Option B)[(https://theworldsgonemad.net/2021/2022/mpls-vpn-optionb/)]. The lab is built in EVE-NG using the following devices and images, username and password are *admin* and *Pa$$w0rd*

- **WAN01, WAN02, CORE01:** *CSR using IOS-XE 15.6(1)S4*
- **DC1, DC2:** *IOS router using IOSv 15.6(2)T*

The packet capture shows MPLS header in the ICMP Packets (wireshark filter *icmp*) as well as BGP updates advertising the label (wireshark filter *bgp.type == 2*)
