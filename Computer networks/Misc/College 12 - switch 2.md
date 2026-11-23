Press RETURN to get started!

  

  

%LINK-5-CHANGED: Interface GigabitEthernet0/1, changed state to up

  

%LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/1, changed state to up

  

%LINK-5-CHANGED: Interface FastEthernet0/3, changed state to up

  

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/3, changed state to up

  

%LINK-5-CHANGED: Interface FastEthernet0/4, changed state to up

  

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/4, changed state to up

  

%LINK-5-CHANGED: Interface FastEthernet0/15, changed state to up

  

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/15, changed state to up

  

%LINK-5-CHANGED: Interface FastEthernet0/16, changed state to up

  

%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/16, changed state to up

  

  

Switch>

Switch>enable

Switch#conf t

Enter configuration commands, one per line. End with CNTL/Z.

Switch(config)#vlan 11

Switch(config-vlan)#name students

Switch(config-vlan)#vlan 22

Switch(config-vlan)#name teachers

Switch(config-vlan)#vlan 99

Switch(config-vlan)#vlan unused

^

% Invalid input detected at '^' marker.

Switch(config-vlan)#name unused

Switch(config-vlan)#exit

Switch(config)#show

^

% Invalid input detected at '^' marker.

Switch(config)#exit

Switch#

%SYS-5-CONFIG_I: Configured from console by console

conf t

Enter configuration commands, one per line. End with CNTL/Z.

Switch(config)#show

^

% Invalid input detected at '^' marker.

Switch(config)#show

Switch(config)#show

Switch(config)#show

Switch(config)#int

Switch(config)#interface range Fa0/1-10

Switch(config-if-range)#sw

Switch(config-if-range)#switchport

Switch(config-if-range)#switchport acc

% Incomplete command.

Switch(config-if-range)#sw

Switch(config-if-range)#switchport mode acc

Switch(config-if-range)#switchport mode access

Switch(config-if-range)#switchport access vklan 22

^

% Invalid input detected at '^' marker.

Switch(config-if-range)#switchport access vlan 22

Switch(config-if-range)#inter

Switch(config-if-range)#interface range Fa0/13-22

Switch(config-if-range)#switchport mode access

Switch(config-if-range)#switchport access vlan 11

Switch(config-if-range)#exit

Switch(config)#interface range fa0/11-13, fa0/23-24, Gig0/0

interface range not validated - command rejected

Switch(config)#switchport access vlan 11

^

% Invalid input detected at '^' marker.

Switch(config)#switchport mode access

^

% Invalid input detected at '^' marker.

Switch(config)#show interface

^

% Invalid input detected at '^' marker.

Switch(config)#show interfaces

^

% Invalid input detected at '^' marker.

Switch(config)#sh int

^

% Invalid input detected at '^' marker.

Switch(config)#sh int tr

^

% Invalid input detected at '^' marker.

Switch(config)#do show vlan brief

  

VLAN Name Status Ports

---- -------------------------------- --------- -------------------------------

1 default active Fa0/11, Fa0/12, Fa0/23, Fa0/24

Gig0/1, Gig0/2

11 students active Fa0/13, Fa0/14, Fa0/15, Fa0/16

Fa0/17, Fa0/18, Fa0/19, Fa0/20

Fa0/21, Fa0/22

22 teachers active Fa0/1, Fa0/2, Fa0/3, Fa0/4

Fa0/5, Fa0/6, Fa0/7, Fa0/8

Fa0/9, Fa0/10

99 unused active

1002 fddi-default active

1003 token-ring-default active

1004 fddinet-default active

1005 trnet-default active

Switch(config)#interface Gig0/1

Switch(config-if)#switchport mode trunk

  

Switch(config-if)#

%LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/1, changed state to down

  

%LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/1, changed state to up

switchport trunk native vlan99

^

% Invalid input detected at '^' marker.

Switch(config-if)#

Switch(config-if)#

Switch(config-if)#

Switch(config-if)#

Switch(config-if)#switchport trunk native vlan 99

Switch(config-if)#exit

Switch(config)#exit

Switch#

%SYS-5-CONFIG_I: Configured from console by console

  

Switch#show vlan

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

  

VLAN Name Status Ports

---- -------------------------------- --------- -------------------------------

1 default active Fa0/11, Fa0/12, Fa0/23, Fa0/24

Gig0/2

11 students active Fa0/13, Fa0/14, Fa0/15, Fa0/16

Fa0/17, Fa0/18, Fa0/19, Fa0/20

Fa0/21, Fa0/22

22 teachers active Fa0/1, Fa0/2, Fa0/3, Fa0/4

Fa0/5, Fa0/6, Fa0/7, Fa0/8

Fa0/9, Fa0/10

99 unused active

1002 fddi-default active

1003 token-ring-default active

1004 fddinet-default active

1005 trnet-default active

  

VLAN Type SAID MTU Parent RingNo BridgeNo Stp BrdgMode Trans1 Trans2

---- ----- ---------- ----- ------ ------ -------- ---- -------- ------ ------

1 enet 100001 1500 - - - - - 0 0

11 enet 100011 1500 - - - - - 0 0

22 enet 100022 1500 - - - - - 0 0

99 enet 100099 1500 - - - - - 0 0

1002 fddi 101002 1500 - - - - - 0 0

1003 tr 101003 1500 - - - - - 0 0

1004 fdnet 101004 1500 - - - ieee - 0 0

1005 trnet 101005 1500 - - - ibm - 0 0

  

VLAN Type SAID MTU Parent RingNo BridgeNo Stp BrdgMode Trans1 Trans2

---- ----- ---------- ----- ------ ------ -------- ---- -------- ------ ------

  

Switch#show

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

% Incomplete command.

Switch#show interfaces trunk

Port Mode Encapsulation Status Native vlan

Gig0/1 on 802.1q trunking 99

  

Port Vlans allowed on trunk

Gig0/1 1-1005

  

Port Vlans allowed and active in management domain

Gig0/1 1,11,22,99

  

Port Vlans in spanning tree forwarding state and not pruned

Gig0/1 1,11,22,99

  

Switch#

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

%CDP-4-NATIVE_VLAN_MISMATCH: Native VLAN mismatch discovered on GigabitEthernet0/1 (99), with Switch GigabitEthernet0/2 (1).

  

Switch#