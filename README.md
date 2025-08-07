# Basic Lan Setup with Cisco Packet Tracer Home lab<br>
<img width="748" height="526" alt="image" src="https://github.com/user-attachments/assets/cfb88876-5e85-4ab4-9b9f-6e132007a2e5" /><br>

# Technology Utilized
- CISCO Packet Tracer
- Routers
- Switches
- DHCP

## Objective: To simulate a small office network with three wired computers, one printer, and a wireless laptop, all connected to the same LAN. The router will provide DHCP to all devices, and you will test connectivity between them.

### Activity 1: Basic Lab Setup
#### From the End Devices section and the Network Devices section, drag and drop:
- 3 PCs (PC-0, PC-1, PC-2), 1 Laptop (Laptop-0), 1 Printer (Printer-0)
- 1 Router (Router-0), 1 Switch (Switch-0), 1 Wireless Router (WirelessRouter-0) <br>

<img width="530" height="273" alt="image" src="https://github.com/user-attachments/assets/8927726a-bf80-4b95-9d2d-a9d1c49c2d4f" /><br>

#### Wired and Wireless Connections:
- Connect each PC to the Switch using the copper straight-through cable.
  - PC-0 to FastEthernet 0/1, PC-1 to FastEthernet 0/2, PC-2 to FastEthernet 0/3.
- Connect the Printer to the Switch (FastEthernet 0/4).
- Connect the Router to the Switch using a straight-through cable 
  - Router's GigabitEthernet 0/0 to Switch’s FastEthernet 0/5.
- Connect WirelessRouter-0 to the Router by using a crossover cable.
  - WirelessRouter-0’s Internet port to Router’s GigabitEthernet 0/1.<br>
  
 <img width="524" height="371" alt="image" src="https://github.com/user-attachments/assets/7b28c8fb-cb35-4150-80fc-67ec937f56bd" /><br>

### Activity 2: Router Configurations
#### Configure the Router’s GigabitEthernet 0/0 interface and GigabitEthernet 0/1 interface (WirelessRouter-0):<br>
<img width="695" height="498" alt="image" src="https://github.com/user-attachments/assets/c6356c7e-7f06-4fac-a74d-65e79d649e88" />
<img width="579" height="407" alt="image" src="https://github.com/user-attachments/assets/abd77b3c-39b4-47e5-a943-0a4a2eae949a" /><br>

#### Set up a DHCP Pool for wired devices on the 192.168.1.0/24 network and wireless devices on the 192.168.2.0/24 network:<br>
<img width="841" height="314" alt="image" src="https://github.com/user-attachments/assets/7a559a23-8da0-4325-b838-092bb253fa18" /><br>
#### DHCP proper IP address assignment verification:<br>
<img width="646" height="262" alt="image" src="https://github.com/user-attachments/assets/40c8c624-c1bc-4ffd-87c8-265e666817c6" />
<img width="689" height="251" alt="image" src="https://github.com/user-attachments/assets/2ce7d00b-2d23-4d4d-8c7f-c25c43dd3ffb" /><br>

### Activity 3: Wireless Router Configurations
- Set the Internet IP Addressand Subnet Mask.
<img width="828" height="537" alt="image" src="https://github.com/user-attachments/assets/1ccee286-7167-4bb1-8a15-8dc29c3eb290" /><br>
- Change the SSID(OfficeWifi) and set WPA2-PSK security and create a passphrase.<br>
<img width="841" height="369" alt="image" src="https://github.com/user-attachments/assets/cc02d2ec-a5ff-45c7-9f23-7e3acc985192" />
<img width="834" height="323" alt="image" src="https://github.com/user-attachments/assets/24442e3f-418f-4c28-b602-04cdbe933946" /><br>

- Connect the Laptod to the office Wifi and check of WPA2-PSK verificatino:<br>
<img width="556" height="385" alt="image" src="https://github.com/user-attachments/assets/0dbd4abe-428c-49d4-a9fa-29a9af3f11b0" />
<img width="497" height="375" alt="image" src="https://github.com/user-attachments/assets/2bb9ac75-204a-4cf7-8197-7ced7c88953f" />
<img width="748" height="526" alt="image" src="https://github.com/user-attachments/assets/cfb88876-5e85-4ab4-9b9f-6e132007a2e5" /><br>

### Activity 4: Printer Setup
#### Choose a Static IP Address (Assign outside of DHCP pool)
#### Default Gateway: The IP of the router, which is 192.168.1.1 (the router that serves as the default gateway for the wired LAN).
#### DNS Server: Same IP as the default gateway (192.168.1.1). Can also be a public DNS server (8.8.8.8).<br>
<img width="804" height="444" alt="image" src="https://github.com/user-attachments/assets/18f5b9fd-97b6-4b6b-a31b-e9cbcd94d198" /><br>

#### Test Connectivity to the Printer:<br>
<img width="831" height="365" alt="image" src="https://github.com/user-attachments/assets/c45dd78b-d3f8-45cf-8e85-e0a091bd8373" /><br>
