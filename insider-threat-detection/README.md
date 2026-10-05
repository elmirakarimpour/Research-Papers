# Unsupervised Insider Threat Detection Using BiLSTM-Based Deep Clustering

*Elmira Karimpour — Shiraz University*

**Status:** Manuscript in preparation. Based on my ongoing Master's thesis.

## Abstract

Insider threats pose a significant challenge to organizational cybersecurity due to the difficulty of distinguishing malicious activities from legitimate user behavior. Unlike conventional intrusion detection approaches that often rely on predefined attack patterns or labeled data, insider threat detection requires models capable of identifying subtle and previously unseen behavioral anomalies. This study proposes an unsupervised framework based on Bidirectional Long Short-Term Memory (BiLSTM) networks and deep clustering to learn meaningful representations of user behavior sequences and identify anomalous activity without relying on predefined attack labels. By combining sequential representation learning with clustering-based anomaly detection, the proposed approach aims to capture complex temporal patterns in user behavior and improve the detection of previously unknown insider threats. The framework is evaluated on user activity data to assess its effectiveness in distinguishing anomalous behaviors from normal activity.

## Introduction

Insider threat detection is challenging because malicious user behavior is rare, difficult to label reliably, and highly imbalanced relative to normal activity. These characteristics make approaches that depend heavily on labeled attack examples difficult to apply in realistic settings.

This research investigates an unsupervised approach for learning meaningful representations of user behavior from behavioral sequences without relying entirely on labeled malicious examples.

## Problems we address

1. **Highly imbalanced behavioral data.** Malicious behavior represents only a small portion of user activity, making reliable detection difficult.
2. **Limited reliable malicious examples.** How can meaningful behavioral patterns be learned when trustworthy examples of malicious activity are scarce?
3. **Learning and analyzing behavioral representations.** How can learned representations capture meaningful deviations from normal user behavior while preserving informative patterns?

## Our approach, in brief

The proposed framework models user activities as behavioral sequences and uses a BiLSTM Autoencoder to learn behavioral representations. A learnable user embedding is incorporated to capture user-specific context, while a Contrastive Learning objective encourages more informative representations. Deep Clustering is then used to analyze the learned representation space and identify deviations from normal behavioral patterns.

The deep-learning pipeline is implemented and trained using PyTorch, while scikit-learn is used for data analysis, evaluation, and comparison with conventional machine-learning methods.

## Research focus

A central focus of this work is understanding how different learning components influence the quality and stability of learned representations, particularly in highly imbalanced settings where frequent patterns may dominate learning while rare but important patterns receive less attention.

## Manuscript

*Unsupervised Insider Threat Detection Using BiLSTM-Based Deep Clustering*

The manuscript is currently in preparation as part of my ongoing Master's thesis. The complete manuscript, detailed experimental results, and implementation are not publicly available at this stage.