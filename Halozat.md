# Hálozat Commandok

## SSH 

    Router> ena
    Router# conf t
    Router(conf)# hostname R1
    R1(conf)# ip domain-name petrik.hu
    R1(conf)# crypto key generate RSA
    RSA: 1024
    R1(conf)# username Preisler password/secret Kód
    R1(conf)# ip ssh version 2
    R1(conf)# line vty 0 15
    R1(line)# login local
    R1(line)# transport input ssh

## IPv6

    Router> ena
    Router# conf t
    Router(conf)# ipv6 unicast-routing
    Router(conf)# int g0/0
    Router(int)# ipv6 address 2001:DA48:FC5:A4:A::/64
    Router(int)# ipv6 address FE80::1 link-local
    Router(int)# no sh

## VLSM

    254host => /24 == 255.255.255.0
    126host => /25 == 255.255.255.128
    62host  => /26 == 255.255.255.192
    30host  => /27 == 255.255.255.224
    14host  => /28 == 255.255.255.240
    6host   => /29 == 255.255.255.248
    2host   => /30 == 255.255.255.252

    
    