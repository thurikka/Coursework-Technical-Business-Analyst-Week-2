# Phase 1 Scope — Smart-Recovery Portal

## In scope

- **Identity verification (secure login, document upload, and manual verification support)**
  *Justification:* Replaces fragmented email-based document submission with a structured intake flow in the portal. This reduces operational inefficiency, improves traceability, and maintains compliance by keeping verification agent-led.

- **Account summary and eligible actions (balance, breakdown, status, next steps)**  
  *Justification:* Directly addresses the highest-priority customer need of understanding what is owed and what to do next. Reduces repeated customer contact and agent workload.

- **Promise-to-Pay (PTP) capture and tracking with basic eligibility rules**  
  *Justification:* Improves follow-up consistency and reduces missed recovery opportunities. Replaces unreliable manual tracking with structured commitments.

- **Eligible repayment options display (selection only, no payment execution)**  
  *Justification:* Enables customer self-service while avoiding the complexity and risk of handling payments in Phase 1.

- **Rules-based routing to agents for complex or ineligible cases**  
  *Justification:* Ensures high-risk and complex cases remain human-led, maintaining compliance and operational trust while allowing safe automation of straightforward cases.

- **Automated follow-up scheduling for PTP and missed actions**  
  *Justification:* Directly addresses revenue leakage caused by missed follow-ups and reduces reliance on manual tracking.

- **Audit logging and structured event tracking across customer journeys and financial state changes**
  *Justification:* Captures key customer actions (e.g. login, account view, PTP creation) and financial state changes (e.g. payment received, delinquency updates). This ensures end-to-end traceability for compliance, operational oversight, and performance measurement. It supports a consistent view of activity across fragmented systems without duplicating existing data sources or creating a new system of record.

- **Lightweight unified agent view (account summary, PTP status, activity history)**  
  *Justification:* Reduces time spent reconciling fragmented systems, improving agent efficiency without requiring full system replacement.

- **Basic portal outcome reporting (self-service usage, PTP rates, follow-up completion)**  
  *Justification:* Provides visibility into whether the portal is reducing workload and improving recovery performance.

---

## Out of scope

- **Hardship assessment or vulnerability detection automation**  
  *Justification:* Requires sensitive human judgment and carries high compliance risk. Better handled through agent review.

- **Abusive behaviour detection or escalation automation**  
  *Justification:* Difficult to reliably automate and risks incorrect handling of sensitive situations.

- **Legal escalation workflows and enforcement actions**  
  *Justification:* High-risk, low-volume processes that would significantly increase complexity without contributing to Phase 1 value.

- **Full replacement of the legacy collections platform**  
  *Justification:* Not feasible within Phase 1. A layered approach reduces delivery risk and enables incremental improvement.

- **AI-driven prioritisation or predictive decisioning**  
  *Justification:* Requires high-quality data and explainability. Not necessary to achieve early value and may reduce stakeholder confidence.

- **Payment processing or funds transfer within the portal**  
  *Justification:* Introduces regulatory and technical complexity. Phase 1 focuses on commitment capture rather than transaction execution.

- **Bespoke repayment negotiation flows**  
  *Justification:* Complex and variable, requiring human judgment. Not suitable for initial rules-based automation.

- **Advanced personalisation or recommendation engines**  
  *Justification:* Lower immediate value compared to core functionality and adds unnecessary complexity for Phase 1.

---

## Assumptions

- Legacy systems can provide sufficient data for account summary and status display  
- Eligibility rules for PTP and routing can be agreed without full policy redesign  
- Operations teams will continue handling complex and high-risk cases  
- A pilot or phased rollout approach is acceptable  
- Customers can be reliably identified and authenticated  
- Compliance requirements can be met with audit logging and limited financial action scope  

---

## Dependencies and constraints

- Integration with legacy collections systems for account data  
- Agreement on PTP eligibility rules (e.g. blocked accounts, frozen funds, accounts heavily overdrawn)  
- Compliance approval for identity verification, audit logging, and messaging  
- Alignment with agent workflows for routed cases  
- Data quality limitations in existing systems  
- Clear ownership between portal and existing tools to avoid duplication  

---

## Why this scope is credible

This scope directly targets the highest-impact issues identified in discovery: reducing repeated customer contact, improving follow-up reliability, and reducing agent time spent reconciling fragmented systems. By focusing on account clarity and structured Promise-to-Pay capture, it addresses both customer friction and key drivers of revenue leakage.

The scope is deliberately constrained to a focused, high-value set of capabilities. It avoids complex, high-risk areas such as legal workflows and hardship assessment, while introducing a self-service layer that complements rather than replaces existing systems. This supports a phased delivery approach, allowing value to be delivered early while reducing integration and adoption risk.

By maintaining clear handoffs to agents for complex or high-risk cases and limiting automation to rules-based scenarios, the solution balances efficiency gains with operational control and compliance confidence. This ensures the system can be adopted incrementally, with performance and impact measured and refined before expanding scope in later phases.