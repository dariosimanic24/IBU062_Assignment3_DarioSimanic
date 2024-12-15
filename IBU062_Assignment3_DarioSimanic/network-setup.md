Router: Cisco 1841
Switch1: Cisco 2960
Switch2: Cisco 2960
Laptop1: 168.90.0.2 (Switch 1)
PC1: 168.90.0.3 (Switch 1)
PC2: 168.90.0.4 (Switch 1)
Server1: 168.90.0.5 (Switch 1)
PC3: 210.3.14.2 (Switch 2)
Server2: 210.3.14.4 (Switch 2)
Server3: 210.3.14.3 (Switch 2)
PC4: 168.90.0.6 (Switch 1)
PC5: 210.3.14.5 (Switch 2)


DHCP Configuration on the Router

For Switch 1
ip dhcp pool FIRST_NETWORK
network 168.90.0.0 255.255.0.0
default-router 168.90.0.1
exit

ip dhcp pool SECOND_NETWORK
network 210.3.14.0 255.255.255.0
default-router 210.3.14.1
exit
