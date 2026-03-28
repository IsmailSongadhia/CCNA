# Small Network Router Configuration - Cyber Security Project

This project demonstrates how to create and configure a small local area network (LAN) using a router and multiple PCs. It covers basic router configuration, IP addressing, subnetting, and network connectivity testing — an essential practical for Cyber Security, Networking, and Computer Science students.

## 📋 Project Overview

The goal of this project is to:
- Set up a basic router with proper IP configuration
- Assign static IP addresses to PCs in the same subnet
- Configure default gateway and DNS
- Verify network connectivity between PCs and the router using ping

### Tools & Requirements
- Packet Tracer (or any network simulator)
- Router (e.g., 2811 or 4331 in Packet Tracer)
- 2 or more PCs
- Console cable (for initial router configuration)

## 📷 Project Screenshots

(Replace these with your actual screenshot links after uploading images to your GitHub repo)

![Network Topology](images/image1.png)
*Network Topology in Packet Tracer*

![Router Configuration](images/image2.png)
*Router CLI Configuration Steps*

## 🚀 Step-by-Step Configuration Guide

### Step 1: Router Configuration (CLI)

1. Open Packet Tracer
2. Add a router (e.g., 2811) and connect it to PCs using crossover or straight-through cables
3. Click on the router → **CLI** tab
4. Enter the following commands:

```bash
Router> enable
Router# configure terminal
Router(config)# hostname R1     (optional - give a name)

Router(config)# interface GigabitEthernet0/0
Router(config-if)# ip address 10.0.0.1 255.255.255.0
Router(config-if)# no shutdown
Router(config-if)# exit
