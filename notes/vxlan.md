# VXLAN Overview

VXLAN (Virtual Extensible LAN) is used in ACI as the overlay technology.

## Key Concepts

- Encapsulation of Layer 2 frames into UDP packets
- Uses VTEPs (VXLAN Tunnel Endpoints)
- Allows Layer 2 extension over Layer 3 networks

## In this Lab

- Leaf switches act as VTEPs
- Traffic between hosts is encapsulated using VXLAN
- Spine acts as the underlay transport

## Why VXLAN?

- Scalability beyond VLAN limits
- Network segmentation
- Multi-tenant environments
