# rand_ip

# Information #

Random IPv4 address and CIDR mask generator. Generates CIDR masks covering the range of 16-30 through IPv4 Classes A-E
Can be utilized while studying subnetting in order to generate random IP addresses along with subnet masks to work out:
1. Network the IP address is in
2. Next network address
3. Usable IP range within network
4. Broadcast address
5. Number of hosts available

Tool was initially developed while studying for CompTIA Network+ exam - hence can be used by those wanting to practice 
subnetting with CIDR mask. The reason behind only providing CIDR masks for the last two octets is the certification
generally only covered those

# Usage #
./rand_ip.sh -a 2
This will generate two random Class A addresses

Flags can be added on as follows:
./rand_ip.sh -a 2 -c 2 -d 2 -b 2

Utilizing the -q option will remove the headers generated otherwise (header info provides class & number of IPs generated)
./rand_ip.sh -q -a 1 -c 1 -d 1 -b 1
