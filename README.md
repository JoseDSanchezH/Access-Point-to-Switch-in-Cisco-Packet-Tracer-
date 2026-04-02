# Access-Point-to-Switch-in-Cisco-Packet-Tracer



## Overview 

When you connect your laptop to the office Wi-Fi and send a file to someone sitting at a desk computer that's plugged directly into the wall, how does that actually work? Those two devices are on completely different types of connections. 1 is wireless, one is wired. Yet somehow they communicate instantly. 

In this lab, I will demonstrate how to build that in a small network that connects wireless devices through an access point to wired devices connected through a switch by simulating the kind of hybrid network infrastructure found in virtually every modern office, school, and retail environment.

# Steps Taken 

1. Rather than starting from scratch, I expanded my previous wireless lab environment, which already has an access point, a wireless laptop, a wireless PC, and a smartphone connected. To simulate the hybrid office network, I will add a network switch, which is a device that manages wired connections and allows multiple devices to communicate on the same network. And I will add 2 desktop PCs, PC #1 and PC #2, connected to the switch via Ethernet cables.

A switch handles local device-to-device communication efficiently. A router handles traffic going outside the network they both have different jobs.

I then connected the access points directly into the switch, which allows wireless devices and wired devices to talk to each other. Think of the switch as the central hub of the office; every device, whether plugged into it or connected wirelessly, eventually routes its traffic through it.

<img width="1270" height="586" alt="image" src="https://github.com/user-attachments/assets/e811b5e2-d825-4e8f-a779-42d2bcd08dd8" />



2. I now need to enable port 0 on the access point. In my previous lab, I made sure to turn this on just in case I were to do this lab. It never hurts to check because you can overlook things in a real environment. Port one handles wireless connections, which is what I connected my phone, laptop, and computer to the access point. Port 0 handles the wired connection back to the switch.


<img width="1132" height="454" alt="image" src="https://github.com/user-attachments/assets/0509944f-92fb-4150-bbff-549341c6699b" />


3. Every device on a network needs a unique address so the information knows exactly where it's going to go. I will be using the same static IP address, meaning I will manually assign each device its own permanent address rather than having a server assign them automatically.

PC 1: 192.168.1.5
PC 2: 192.168.1.6

It will automatically assign the subnet mask of 255.255.255.0

<img width="1314" height="676" alt="image" src="https://github.com/user-attachments/assets/9efae242-cdd4-42a4-bff9-c84f7ad86346" />


<img width="1178" height="580" alt="image" src="https://github.com/user-attachments/assets/afc408f7-93b0-4122-bcbc-b84b8b393789" />



4. This is where the lab proves its point because I will send test packets, called a ping, from the wireless laptop connected to the access point addressed to PC #1, which is plugged in directly into the switch via Ethernet cable.

Below are the screenshots I captured showing step by step how the data packet travels its full journey across the network.

<img width="1074" height="454" alt="image" src="https://github.com/user-attachments/assets/2082e20a-cfd4-4343-96ce-08458cdb9d7d" />

<img width="950" height="450" alt="image" src="https://github.com/user-attachments/assets/dc9c0f81-7387-414c-8095-6e07d61281c4" />


<img width="1096" height="482" alt="image" src="https://github.com/user-attachments/assets/a7338fbd-16e0-4087-b986-9652b87abb55" />

<img width="1098" height="466" alt="image" src="https://github.com/user-attachments/assets/fef843cf-72f0-4504-a599-abe3f229f34c" />

<img width="1058" height="486" alt="image" src="https://github.com/user-attachments/assets/25664ad4-dd0a-4b59-8720-dd2c5d06ed5d" />






