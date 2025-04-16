# AS1273 Junos Evo Topology

## Overview

AS1273 is a global transit network designed with an iBGP mesh architecture.  

Currently, the network operates without hierarchy, employing a flat structure that has proven effective over time. The design leverages:

- **IS-IS** as the IGP
- **iBGP Mesh**
- **MPLS LSPs**, carrying traffic between nodes, where every node acts as a PE due to the geographically dispersed nature of the network.

The existing infrastructure is based on **MX960**, **MX480**, and **PTX5K** platforms.  

This repository contains a **VMM configuration** replicating the current network topology and introduces the **PTX10K platform** running **Junos-Evo** to test advanced features.

---

## Features to Test
The following features are targeted for validation in this topology:

- **BGP**
- **BGP FlowSpec**
- **BGP Optimal Route Reflection (ORR)**
- **IS-IS**
- **MPLS**
- **Interface Group Tag Using Firewall**
- **NetFlow**
- **PCEP**
- **RIB Group**
- **RSVP-TE**
  - **RSVP-TE ERO**
  - **RSVP-TE FRR (Node-Link Protection)**
- **SNMPv3**
- **TWAMP**
- **Telemetry (OpenConfig)**
- **Apply-Groups**
- **Segment Routing**
- **Streaming Telemetry (gRPC and gNMI)**

Introduction of Paragon 2.4 as an SDN controller to satisfy the following use cases. 

      1. Observability
      2. Network Optimization
      3. SLA Platform. 

---

## Topology Diagram

The topology diagram below provides a visual reference for replicating the Junos-Evo network setup:

![image](https://github.com/user-attachments/assets/56ee9cc0-3980-4d1a-9602-707690dbe156)


---

## Platforms Used

- **Current Setup**: MX960, MX480, PTX5K
- **New Addition**: PTX10K (Junos-Evo)

---

