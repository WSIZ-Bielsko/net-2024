# Layer 2 - RouterOS (v7)

- "switches"
- cheap 10G+ speeds

## Basics

- interfaces
- bridges 
- MAC addresses (and to/from traffic)

- creating a bridge and adding interaces
```
/interface/bridge/add name=b1
/interface/bridge/port/add interface=ether1 bridge=b1
/interface/bridge/port/add interface=ether2 bridge=b1
/interface/bridge/port/add interface=ether3 bridge=b1
/interface/bridge/port/add interface=ether4 bridge=b1
/interface/bridge/port/add interface=ether5 bridge=b1
/interface/bridge/port/add interface=ether6 bridge=b1
```

## STP

## VLAN

## Bonding



