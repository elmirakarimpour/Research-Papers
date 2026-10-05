# CARE-IPS

**A Correlation-Aware, Evidence-Grounded Multi-Agent LLM Framework for Safe Intrusion Detection and Prevention**

*Elmira Karimpour, Mehdi Moghimi, Seyedreza Taghizadeh — Shiraz University*

**Status:** Final evaluation stage.

## Abstract

Multi-agent intrusion detection systems increasingly combine heterogeneous detectors with large language models to improve both detection coverage and interpretability of security decisions. Trustworthy autonomous prevention, however, remains an open problem, since agents that share models, features, or data sources can produce confident agreement that is not truly independent, and language model generated explanations or actions can appear reasonable while being unsupported by the underlying evidence. This paper presents CARE-IPS, a correlation aware, evidence grounded multi agent framework for safe intrusion detection and prevention. Heterogeneous detection agents report calibrated confidence and faithfulness validated evidence, a correlation aware consensus mechanism discounts agreement that is not independently supported, a bounded reasoning agent generates mitigations that cite only validated evidence, and a deterministic safety gate authorizes autonomous action only when evidence sufficiency, independent support, policy compliance, and reversibility are jointly satisfied. Compared with majority voting and existing explainable detection approaches, the proposed framework is designed to reduce unsafe or unnecessary autonomous actions and to lower the rate of undetected coordinated attacks that arise from correlated agent agreement, while preserving detection accuracy comparable to unconstrained baselines.



## Introduction

Modern AI-based intrusion detection systems can reach high detection accuracy, and multi-agent and LLM-based systems now add collaborative analysis and human-readable explanations. Letting such systems take *autonomous preventive action* is a different matter: a wrong action can disrupt legitimate services instead of stopping an attack.

## Problems we address

1. **Agreement is not always independent evidence.** When several detection agents share models, features, data or prompts, they can confidently repeat the same mistake. Treating their agreement (for example, a majority vote) as trustworthy hides this shared blind spot.
2. **Plausible is not the same as supported.** An LLM-generated explanation or mitigation can sound reasonable while not being grounded in the evidence the detectors actually produced.
3. **Autonomy needs accountability.** Before any action is taken, it should be traceable to evidence, within policy, bounded in risk and reversible.

## Scope

This work does not propose a new detection model or a new explanation technique. It focuses on the decision layer that sits between multiple, possibly correlated detectors and an autonomous response, which existing multi-agent and explainable intrusion detection systems tend to leave unexamined.

## Our approach, in brief

CARE-IPS is a framework for turning evidence from several detection agents into safe, auditable autonomous decisions, escalating to a human analyst when that cannot be justified. Architecture details, evaluation setup and results will be made public after publication.

## Full manuscript

Available on request: elmirakarimpour@outlook.com
