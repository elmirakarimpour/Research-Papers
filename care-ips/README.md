# CARE-IPS

**A Correlation-Aware, Evidence-Grounded Multi-Agent LLM Framework for Safe Intrusion Detection and Prevention**

*Elmira Karimpour, Mehdi Moghimi, Seyedreza Taghizadeh — Shiraz University*

**Status:** Final evaluation stage.

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

Available on request: e.elmirakarimpour@gmail.com
