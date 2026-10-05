# TwinFL-R

**A Cyber Twin–augmented federated Random Forest framework for IoT intrusion detection**

*Elmira Karimpour, Mehdi Moghimi, Seyedreza Taghizadeh — Shiraz University*

**Status:** Under review, 6th International Conference on Computing and Machine Intelligence (ICMI) 2027, Mount Pleasant, Michigan, USA.

## Abstract

The rapid proliferation of Internet‑of‑Things (IoT) devices with constrained processing capabilities has exposed new attack surfaces and challenged the viability of centralized intrusion detection systems (IDS). Cloud‑centric models require transmitting raw traffic to a remote server, introducing latency, bandwidth overhead and privacy risks. This paper proposes TwinFL‑R, a lightweight federated learning architecture for IoT intrusion detection that combines Random‑Forest classifiers with edge‑deployed Cyber Twins. Each IoT node and its Cyber Twin collaboratively train a local Random‑Forest model using real network traces and synthetically generated attack scenarios; only serialized decision‑trees are uploaded to a central aggregator. The aggregator employs a tree‑selection strategy that retains the most discriminative trees to form a compact global ensemble, eliminating the need for parameter averaging. Experiments on the CIC‑IDS2017 dataset under non‑IID partitions demonstrate that TwinFL‑R achieves 96.7 % accuracy and a 2.1 % false‑positive rate, while reducing communication and computational overhead relative to centralized CNN/RNN and standalone Random‑Forest baselines. The results indicate that the proposed framework enhances detection precision and resilience while minimizing raw data exposure, making it well suited for large‑scale, privacy‑aware IoT deployments.      
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
