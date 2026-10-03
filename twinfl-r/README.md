# TwinFL-R

**A Cyber Twin–augmented federated Random Forest framework for IoT intrusion detection**

*Elmira Karimpour, Mehdi Moghimi, Seyedreza Taghizadeh — Shiraz University*

**Status:** Under review, 6th International Conference on Computing and Machine Intelligence (ICMI) 2027, Mount Pleasant, Michigan, USA.

## Introduction

The number of Internet-of-Things (IoT) devices keeps growing, and so does the attack surface they expose. Most intrusion detection systems (IDS) still follow a centralized design: raw network traffic is sent to a remote server for analysis. For IoT deployments this creates three practical problems: latency and bandwidth cost, exposure of potentially sensitive traffic data, and a single point of failure.

## Problems we address

1. **Privacy and communication.** How can devices contribute to a shared detector without sending raw traffic to a central server?
2. **Resource constraints.** Deep models such as CNNs and RNNs are often too heavy for constrained IoT hardware. Can a lightweight model family be used in a federated setting?
3. **Heterogeneous, imbalanced local data.** Each device sees only part of the traffic, and some attack types are rare or entirely absent locally. How can local models learn to recognize attacks they have rarely or never observed?

## Our approach, in brief

TwinFL-R combines federated learning with lightweight tree-based classifiers and edge-side Cyber Twins that help cover under-represented attack patterns. The design goal is a compact shared model that improves detection while reducing communication and keeping raw data on the device.

The specific mechanisms, experimental setup and results will be made public after publication.

## Limitations we acknowledge

Reduced data exposure is not a formal privacy guarantee, and robustness against malicious participants is left for future work.

## Full manuscript

Available on request: elmirakarimpour@outlook.com
