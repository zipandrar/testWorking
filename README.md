# testWorking
sometimes,,,, it is hard to get a small tip to get it out quickly.... ...some problem's tip...




ubuntu18.04 64bit...  ikev2 ipsec
ipsec up connName

case:
then it will get all traffic to tunnel

want: only route some,not all

way:
ip route show table all
find the line which have "table 220"
ip route del default via 172.17.xxx.xxx dev eth0 table 220 proto static src 172.111.xxx.xxx

result: ok,you can now route only a port traffic to the tunnel ip...with the glider etc...

:)





