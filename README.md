# Aura Sentinel: Agentic Merchant Terminal

## What This Prototype Is
Aura Sentinel is a commercial decision engine prototype designed for enterprise merchants. It transitions the payment dashboard experience from passive data visualization to active, AI-driven orchestration. It uses a multi-agent topology, it autonomously identifies revenue leakage, spots international market growth opportunities, and provides mathematically verified recommendations to deploy Visa Value-Added Services (VAS).

## Tooling & Methodology
This prototype was built using **Hermes** agent.

## Problem Statement
Enterprise merchants face a "cognitive gap" between raw payment telemetry and commercial execution. 
* **Defense (False Declines):** Merchants lose millions to technical friction (e.g., unrecognizable billing descriptors triggering issuing bank fraud models) but lack the analytical bandwidth to diagnose the root cause among millions of ISO-8583 codes.
* **Offense (Market Expansion):** Global merchants miss massive inbound traveler spend surges because their checkout flows are not localized in real-time to support Local Payment Methods (LPMs) or Dynamic Currency Conversion (DCC).

<img width="1691" height="930" alt="image" src="https://github.com/user-attachments/assets/df84382f-8909-4734-b41d-750247840112" />

## Data Ingestion Strategy
The engine is designed to ingest real-time sovereign telemetry rather than delayed batch reports:
1. **Operational Friction:** Real-time ISO-8583 message streams (specifically parsing Field 39 for response codes and Field 43 for merchant descriptors).
2. **Market Opportunity:** Global Geographic BIN (Bank Identification Number) pulses to track high-intent cross-border traveler surges.

## Agentic Architecture
To handle enterprise-scale transaction volume securely, Aura Sentinel utilizes a 4-Agent Topology:
1. **Flux Orchestrator:** The gatekeeper that monitors the raw stream for anomalies and routes them to specialized agents, keeping compute costs lean.
2. **Diagnostic Scout:** The defense agent. Utilizes Retrieval-Augmented Generation (RAG) against an ISO Diagnostic Ledger to identify the root cause of false declines.
3. **Growth Scout:** The offense agent. Cross-references inbound BIN surges against a global LPM registry to identify share-of-wallet gaps.
4. **Sandbox Simulator:** The trust engine. Before surfacing a recommendation, this agent tests the proposed Visa API fix against a shadow ledger of the merchant's last 30 days of transactions to mathematically verify the exact financial ROI.

## User Persona
Designed for the **VP of Payments or Director of Global E-commerce** at a digital-first global merchant (e.g., a SaaS platform, digital retailer, or gaming enterprise). These leaders process massive international volume and need an autonomous system that provides actionable, revenue-recovering strategies rather than just raw decline metrics.

## Business & User Impact
Aura Sentinel aligns product utility with commercial monetization:
* **Business KPI (Merchant):** Increases Total Addressable Market (TAM) capture by recovering technical leakage and bridging localized share-of-wallet gaps.
* **Business KPI (Visa):** Acts as an autonomous sales engine for Visa Value-Added Services (VAS), pitching APIs precisely when the merchant feels the pain of lost revenue.
* **User KPI:** Drastically reduces "Time-to-Insight" from weeks to seconds. By exposing the Agentic "Chain of Thought" and Sandbox Simulation results, it achieves the ultimate user metric in enterprise AI: absolute trust.

<img width="3083" height="1907" alt="image" src="https://github.com/user-attachments/assets/e1e4f4bf-a4da-4378-8086-aefb6d7c1c08" />

<img width="3084" height="1904" alt="image" src="https://github.com/user-attachments/assets/47de8cd1-e2a7-43e7-a61c-7d015a9fe129" />



