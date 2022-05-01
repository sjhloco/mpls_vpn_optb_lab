# MPLS-VPN Option B Lab

The configuration files from a blog post I wrote about [MPLS-VPN Option B (Inter-AS Option B)](https://theworldsgonemad.net/2021/2022/mpls-vpn-optionb/). The lab is built in EVE-NG using the following devices and images with a username and password of ***admin*** and ***Pa$$w0rd***

- **WAN01, WAN02, CORE01:** *CSR using IOS-XE 15.6(1)S4*
- **DC1, DC2:** *IOS router using IOSv 15.6(2)T*

![underlay_and_overlay](https://user-images.githubusercontent.com/33333983/166149141-35377403-46cf-4ea5-b466-f7d783829f53.png)
![blu_vrf](https://user-images.githubusercontent.com/33333983/166149139-9d536fb0-fe87-4d30-98da-711757ec7a08.png)

The packet capture (bgp_update_and_ping_capture.pcapng) shows MPLS header in the ICMP Packets (wireshark filter ***icmp***) as well as BGP updates advertising the label (wireshark filter ***bgp.type == 2***)

<img width="1215" alt="ping_core01_to_wan02" src="https://user-images.githubusercontent.com/33333983/166149143-55f6c800-a23d-4c0c-8e5a-13fe3c2e4bc6.png">
<img width="1211" alt="bgp_update" src="https://user-images.githubusercontent.com/33333983/166149145-df9f9927-fcef-4a20-87d8-332921cf9145.png">
