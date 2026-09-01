# 🌐 SHARP: Scalable Hybrid Adaptive Routing Protocol

## Overview

This project evaluates the limitations of traditional routing protocols—such as RIP, OSPF, IS-IS, and BGP—and introduces **SHARP**, a novel routing architecture[cite: 3]. SHARP is specifically engineered to address the critical challenges of modern networks, including slow convergence times, excessive control message flooding, and security vulnerabilities like route hijacking[cite: 3].

By bridging the gap between link-state reliability and hierarchical scalability, SHARP provides a robust framework for large-scale, dynamic network environments[cite: 3].

## ✨ Core Protocol Features

*   **3-Tier Hierarchical Architecture:** Organizes the network into Local Zones, Regional Backbones, and a Global Core to efficiently limit the scope of link-state flooding[cite: 3].
*   **Composite Routing Metric:** Replaces static metrics with a dynamic cost function evaluating *Delay, Congestion, Hop Count,* and *Security Score*[cite: 3].
*   **Instant Failure Recovery:** Integrates precomputed backup paths into the Link-State Database (LSDB) for immediate localized rerouting during link failures[cite: 3].
*   **Route Proof Authentication (RPA):** Employs cryptographic signatures, route origin certificates, and sequence numbers to actively reject spoofed or tampered routing updates[cite: 3].
*   **Event-Driven Updates:** Triggers network updates only upon topology changes or congestion thresholds, rather than relying on periodic full-table broadcasts[cite: 3].

## 📊 Simulation & Performance

The protocol was rigorously tested against OSPF using a Python and NetworkX simulation environment[cite: 3]. Performance was evaluated across Local Zone, Inter Zone, and Cross Region scenarios under dynamic congestion and backbone failure conditions[cite: 3]. 

**Key Results vs. OSPF:**
*   **Convergence Time:** Achieved approximately 98% faster reconvergence following a backbone link failure[cite: 3].
*   **Routing Overhead:** Reduced control overhead by over 90% due to localized updates and aggregated zone routing[cite: 3].
*   **Packet Loss & RTT:** Maintained significantly lower packet loss and more stable Round Trip Times (RTT) by utilizing immediate backup path activation[cite: 3].

## 👥 Team Contributors

| Name | Index |
| :--- | :--- |
| **A.H.D. Karunanyaka** | 230321P[cite: 3] |
| **H.H. Palihena** | 230458P[cite: 3] |
| **N.P.P. Piyumal** | 230493R[cite: 3] |
| **M.N.N. Shehan** | 230613M[cite: 3] |
