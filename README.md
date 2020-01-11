# ipsweep
IP Address Sweep

A ping sweep or IP address sweep is a method that can establish a range of IP addresses which map to live hosts.

Bash Command:

for ip in `seq 1 254`; do
ping -c 1 $1.$ip | grep "64 bytes" | cut -d " " -f 4 | tr -d ":" &


Syntax: ./ipsweep.sh 192.168.1
