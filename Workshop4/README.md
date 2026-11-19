# Workshop 4 — When “P” Means Two Things

AIML-500 · Machine Learning Fundamentals · Professional Portfolio Artifact 4

[Open The Interactive Lab](https://quiksun.github.io/AI-ML-Professional-Portfolio/Workshop4/hospital-data-readiness.html) · [View The HTML Source](./hospital-data-readiness.html)

## Overview

Two fictional hospitals use the same code, `P`. At Riverbend it means *present*. At Lakeside it means *pending*. If an analyst treats every `P` as present, four unresolved reports become positive training examples.

I adapted the hospital case from **4.3 Data Challenge Scenarios** using concepts from **4.2 Data Challenges In Machine Learning**. The lab follows 18 reports across 12 encounters. Readers can trace a label back to its source and see how a decision about definitions, repeat reports, or timing changes the result.

## Try The Lab

| Data Challenge | What To Try | What To Look For |
| --- | --- | --- |
| **Conflicting Codes** | Select **Raw Import**. Open **Apply The Rules**, then switch to **Site-Specific Codes**. | Lakeside encounter `L01` starts with `P` on day 1. Its label for that report changes from present to pending when the lab uses Lakeside’s dictionary. |
| **Repeat Reports** | Compare **Site-Specific Codes** with **Latest Per Encounter**. | Riverbend reports the same positive finding for `R05` on days 1 and 2. Counting both gives one encounter two votes. |
| **Late Results** | Select **Check The Label**. Switch between **Day 1 Snapshot** and **Latest Per Encounter**. | Riverbend encounter `R03` is pending on day 1. The confirmation arrives on day 3, so it can supply a label for the day 7 snapshot. |

## What Changes By Day 7

| Audit Setup | Unit Counted | Present / Resolved | Share Marked Present |
| --- | --- | ---: | ---: |
| Raw Import | Report | 10 / 16 | 62.5% |
| Site-Specific Codes | Report | 6 / 12 | 50.0% |
| Latest Per Encounter | Encounter | 5 / 11 | 45.5% |

The percentage uses resolved outcomes as its denominator. Under **Latest Per Encounter**, the finding is present in five encounters and ruled out in six. One is still pending. The bars include all 12 encounters so the unresolved case stays visible.

## Why I Selected This Artifact

A project lead seeing 62.5% and 45.5% might ask what changed at the hospitals. Both figures come from the same reports. I selected this case to show how I would explain the difference to a stakeholder and verify it with an analyst. Before training, I would ask each hospital to confirm its code definitions, agree on a reporting cutoff, and review the encounters that still lack a resolved label.

## Running The Lab Locally

Download `hospital-data-readiness.html` and open it in a browser with JavaScript enabled. The HTML includes the fictional records, the audit calculations, and the styling. ChatGPT assisted with developing the lab and drafting this README.
