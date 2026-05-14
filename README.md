
# Using Netcat as a sender and receiver across a network
Setting up a chat line between systems with Netcat and then sending a txt file from one sytem to another
## Outline: Netcat can operate as a sender and receiver of arbitrary data across a network.

Netcat is installed by default on my Kali VM and on my Metasploitable VM which I will be using both in this demonstration

I need to first look up my IP of My kali machine which is 10.0.2.4
<img width="615" height="153" alt="1" src="https://github.com/user-attachments/assets/3f56afba-c628-405d-b691-d10ff3e22fba" />

I'm going to use Netcat to set up a chat line across my network. I'll set up a netcat listener on Kali by using the -l switch and I'll
use the -p option because I'm using port 3232

<img width="202" height="80" alt="2" src="https://github.com/user-attachments/assets/672782c3-1a20-46c3-9aaa-d327ae3b0643" />

Netcat is now listening for data to come in on Port 3232


I'm now on my metasploitable VM.
This system also has netcat installed by default

I can connect to my Kali VM now by typing nc 10.0.2.4 3232

<img width="484" height="98" alt="3" src="https://github.com/user-attachments/assets/a2c52993-38d5-411a-a939-75197a93b89e" />

I have now established a raw data connection. My Kali VM is on the left and the Metasploitable VM is on the right ready to chat.

<img width="680" height="396" alt="4" src="https://github.com/user-attachments/assets/7ebd3d54-d530-4f97-a162-19bcb2980289" />
