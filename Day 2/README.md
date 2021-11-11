## Day 2a [Types of Hackers | Handy commands and actions]

1. [Hacker_Roadmap](https://github.com/sundowndev/hacker-roadmap#wrench-exploitation-tools) (:star: Star this repository for future reference)

2. [Types of Hackers](https://www.malwarefox.com/types-of-hackers/) 

### Handy terminal shortcuts!
* *Ctrl+C* Terminates a job/process
* *Ctrl+Shift+C* Copy
* *Ctrl+Shift+V* Paste

### Keeping system and applications up-to-date

**`sudo apt-get update && sudo apt-get upgrade`** OR **`sudo apt update && sudo apt full-upgrade`**    -> Update the kali repositories

**`sudo apt-get install <application_name>`** -> Install/update git community repositories


### Access privileges
Most Popular command - **`chmod 777 <file>`**   
            
When we want to set permissions, we just add up the number. 
For example, to set the permissions to read and write, we will use ‘6’ (4 + 2) for the permission. 
 
Here are the different permutations:
   * 0 – *no permission*
   * 1 – *EXECUTE*
   * 2 – *WRITE*
   * 3 – *write and execute*
   * 4 – *READ*
   * 5 – *read and execute*
   * 6 – *read and write*
   * 7 – *read, write, and execute*
   
Depending on the permissions you want to grant to the file, you just set the number accordingly.
What about the 3 digits ‘777’? Well, the First digit is assigned to the Owner, the Second digit is assigned to the Group and the Third digit is assigned to the Others. 
**So for a file with ‘777’ permission, everyone can read, write and execute the file.**


## Day 1b [Types of Hackers | Networking]

#### NETWORKING
```
sudo ifconfig 
OR ip -a           // network adapter information (Your machine's IP is visible at eth0)
iwconfig           // wlan adapters information
ping <ip/url>      // ping to check connection and stability
arp -a             // IP address with MAC address
route              //routing table tells you where the traffic exits
netstat -ano       // all open connections and which one is talking from what port number
```

### OSI Model
OSI stands for Open Systems Interconnection.It is a 7 layer architecture with each layer having specific functionality to perform. All these 7 layers work collaboratively to transmit the data from one person to another across the globe. 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/computer-network-osi-model-layers.png" height="300" width="400">

<b>TCP</b> : https   smtp   ftp <br/>
    1. Connection oriented <br/>
    2. Give Response <br/>
    
<b>UDP</b> : dns   ntp <br/>
    1.No response <br/>

_____________Three Way Handshake______________ <br/>
CLIENT  ---------->Server    <br/>
          *syn* <br/>
CLIENT<-----------Server <br/>
          *ack+syn* <br/>
CLIENT----------->Server<br/>
          *ack* <br/>
Connection complete! <br/>
______________________________________________ <br/>

* **Flags** <br/>
FIN - transmission finished <br/>
PSH - send buffer <br/>
URG - important packet <br/>
RST - Reset connection <br/> <br/>

* **Ports**  <br/>
1.Open  - that actively respond to incoming connection <br/>
2.Closed  - that respond but does not have any services running on that port (Firewall not present) <br/>
3.Filtered - (Firewall present) protected and prevents nmap from determining open/closed <br/>
4.Unfiltered  -  nmap can access but cannot determine open/closed <br/>
5.Open-filtered - nmap belives to be open but can not say <br/>
6.Close-filtered - nmap belives to be closed but can not say <br/> <br/>


### Staying Anonymous in Kali Linux
[How to stay anonmous](https://www.youtube.com/watch?v=VZMHfO9rOCg&list=PLBf0hzazHTGOh6JBKc8WkpyuZgDPW6yTk&ab_channel=HackerSploit)

### Other links to refer
[Getting familier with linux commands](https://linuxize.com/post/basic-linux-commands/)

[IPv4](https://www.geeksforgeeks.org/what-is-ipv4/) and [IPv6](https://www.geeksforgeeks.org/what-is-ipv6/)

[Subnetting](https://youtu.be/OqsXzkXfwRw)
