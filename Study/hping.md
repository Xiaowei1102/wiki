hping -i u1 -a 1.1.1.1 192.165.10.100 -s 100 -p 200 -k -d 100 -1


ifconfig  eth7 10.10.168.111	 			把要用到的网卡设置与目的IP一致的网段。
arp -s 10.10.168.152 	00:11:22:33:44:44		建立静态ARP映射，把目的IP与一个MAC地址绑定，就不会发ARP寻找MAC了。
hping -i u1 -a 192.168.252.131 10.10.168.152 -s 100 -p 200 -k -d 100 -2 -c 10  -I eth7