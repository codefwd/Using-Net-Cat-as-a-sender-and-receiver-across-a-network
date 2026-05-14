# Using Netcat as a sender and receiver across a network
Setting up a chat line between systems with Netcat and then sending a txt file from one sytem to another
## Outline: Netcat can operate as a sender and receiver of arbitrary data across a network.

Netcat is installed by default on my Kali VM and on my Metasploitable VM which I will be using both in this demonstration

I need to first look up my IP of My kali machine which is 10.0.2.4
<img width="615" height="153" alt="1" src="https://github.com/user-attachments/assets/3f56afba-c628-405d-b691-d10ff3e22fba" />

I'm going to use Netcat to set up a chat line across my network. I'll set up a netcat listener on Kali by using the -l switch and I'll
use the -p option because I'm using port 3232 
