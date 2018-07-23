# SSH-Network-Configuration
### Overview  
This application will use SSH to connect to the routers from the network built in GNS3 and send the commands defined in the file to each router. To accomplish greater modularity, the application will collect the management IP addresses of the routers from a dedicated file and log in to the devices using credentials stored in another file. This application will also verify if all 3 files exist in the current directory and it will check the IP connectivity to each router via ICMP. This application also makes use of threading, so all the configuration commands to all routers are sent simultaneously and not one after the other.
### Text Files used in the application
The file ssh_ip.txt contains the IP addresses of the routers in the network. The file ssh_userpass.txt contains the username and password which are separated by a comma. The file ssh_commands.txt has the commands that are to be sent to each router.
