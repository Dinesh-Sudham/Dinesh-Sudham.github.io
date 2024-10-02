---
title: 'RDMA Basics'
date: 2024-10-02
permalink: /posts/2012/08/blog-post-4/
tags:
  - cool posts
  - category1
  - category2
---

Remote Direct Memory Access (RDMA) architecture enables efficient data transfer between Compute Nodes (CN) in a High-Performance Computing (HPC) environment. RDMA over Converged Ethernet version 2 (RoCEv2) utilizes a routed IP Fabric as a transport network for RDMA messages. Due to the nature of RDMA packet flow, the transport network must provide lossless, low-latency packet transmission. The RoCEv2 solution uses UDP in the transport layer, which does not handle packet losses caused by network congestion (buffer overflow on switches or on a receiving Compute Node). To avoid buffer overflow issues, Priority Flow Control (PFC) and Explicit Congestion Notification (ECN) are used as signaling mechanisms to react to buffer threshold violations by requesting a lower packet transfer rate. 
