Switch
• (config)# interface vlan 1
• (config-if)# ip address 192.168.1.1 255.255.255.0
• (config-if)# no shutdown
[[College 5]]
Router
- enable
- hostname
- interface gigabitethernet 0/0/1 (based on switch port!)
- ![[Pasted image 20260309141543.png]]
config-if) # ipv6 address fe80::1 link-local

R1#ping fe80::2
-Output interface: Gigabit0/0

startup-config
- This is the saved configuration file that is stored in NVRAM. It contains all the commands that will be used by the device upon startup or reboot. Flash does not lose its contents when the device is powered off.  
running-config
- This is stored in Random Access Memory (RAM). It reflects the current configuration. Modifying a  running configuration affects the operation of a Cisco device immediately. RAM is volatile memory. It loses all of its content when the device is powered off or restarted. To save changes made to the running configuration to the startup configuration file, use the copy running-config startup-config privileged EXEC mode command.

Router = not a lot of ports
Switch = lot of ports
Console cable is able to hard write the switch

From Wikipedia:
![[Pasted image 20260316121947.png]]

write erase (for unplugging)