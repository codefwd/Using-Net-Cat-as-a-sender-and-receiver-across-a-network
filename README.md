
# Using Netcat as a sender and receiver across a network
Setting up a chat line between systems with Netcat.
## Outline: Netcat can operate as a sender and receiver of arbitrary data across a network.

Netcat is installed by default on my Kali and Metasploitable VMs which I will be using both in this demonstration.
I need to first look up my IP on My kali machine which is 10.0.2.4

<img width="615" height="153" alt="1" src="https://github.com/user-attachments/assets/3f56afba-c628-405d-b691-d10ff3e22fba" />

I'm going to use Netcat to set up a chat line across my network. I'll set up a netcat listener on Kali by using the -l switch and I'll
use the -p option because I'm using port 3232

<img width="202" height="80" alt="2" src="https://github.com/user-attachments/assets/672782c3-1a20-46c3-9aaa-d327ae3b0643" />

Netcat is now listening for data to come in on Port 3232


I'm now on my metasploitable VM.
I'm able to enter the **nc** command because this sytem has Netcat installed by default.

I can connect to my Kali VM now by typing its address 10.0.2.4 with the nc command and the port

<img width="484" height="98" alt="3" src="https://github.com/user-attachments/assets/a2c52993-38d5-411a-a939-75197a93b89e" />

I have now established a raw data connection. My Kali VM is on the left and the Metasploitable VM is on the right ready to chat.

<img width="680" height="396" alt="4" src="https://github.com/user-attachments/assets/7ebd3d54-d530-4f97-a162-19bcb2980289" />

Now on my metasploitable VM I'm going to type a message and we will see it displayed on my Kali box

<img width="742" height="272" alt="5" src="https://github.com/user-attachments/assets/b332d621-49cc-46df-a1ba-4164ac55e145" />

<img width="728" height="281" alt="6" src="https://github.com/user-attachments/assets/3c3f9886-88a0-4be4-bc32-ed87228bbefa" />

Then I will type a message on my Kali to be sent to my Metasploitable VM

<img width="897" height="334" alt="7" src="https://github.com/user-attachments/assets/263bd798-b739-4f4a-a27d-cb981006ec95" />


<img width="903" height="274" alt="8" src="https://github.com/user-attachments/assets/d48d7619-2c5e-4d0a-8db9-0e37ce497cac" />

to close the connection:  do a ctl-C

So that concludes the chat portion of Netcat. Look for my other post about sending a text file from one system to another.

