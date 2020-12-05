# sdn-loadbalancer
POX loadbalancer over a custom topology implementing random, round-robin and weighted round robin algorithms

Here load_balancer.py gives you the topology where a controller is implemented as a load balancer and two switches are connected to 18 hosts

ip_loadbalancer.py is used to implement random load balancing

ip_loadbalancer1.py is used to implement round-robin algorithm 

ip_loadbalancer2.py is used to implement weighted round-robin algorithm

# System Information
SDN Controller ~ POX https://github.com/noxrepo/pox

Virtual Network Topology ~ Mininet~ http://mininet.org/

Evaluation ~ Iperf~ https://iperf.fr/

OS ~ Ubuntu 18.04 LTS ~https://ubuntu.com/

# Topology 

![image](https://user-images.githubusercontent.com/22559413/100772413-8786c200-33cd-11eb-820b-70f6653e8474.png)

Here h1,h2,h3 ~ Web servers

sudo ./pox.py log.level --DEBUG misc.ip_loadbalancer --ip=10.0.1.1 --servers=10.0.0.1,10.0.0.2,10.0.0.3

# Results

![image](https://user-images.githubusercontent.com/22559413/101245741-eb1a3380-36dc-11eb-9f5d-a369c21f91c7.png)

BLB - Before Load Balancing                                                                                                                                                          
ALB - After Load Balancing
