# Phase 1 Scope — Smart-Recovery Portal

## In scope

- **Identity verification (secure login, document upload, and manual verification support)**  
  *Justification:* Provides a controlled and auditable replacement for email-based document submission, improving traceability and compliance while keeping verification safely agent-led.

- **Customer account view & self-service actions (account summary, repayment options, Promise-to-Pay capture with basic eligibility rules)**  
  *Justification:* Addresses the core customer need to understand their balance and take action without contacting support, reducing repeat contact and improving recovery efficiency while keeping complex decisions rules-based.

- **Automated follow-up management (PTP tracking and missed action scheduling)**  
  *Justification:* Reduces missed recovery opportunities caused by manual tracking and improves consistency of collections follow-ups, directly addressing revenue leakage.

- **Rules-based routing and escalation to agents (complex, high-risk, or ineligible cases)**  
  *Justification:* Ensures compliance and operational safety by keeping complex and sensitive cases human-led while allowing automation of straightforward journeys.

- **Audit logging and structured event tracking (customer actions and financial state changes)**  
  *Justification:* Enables end-to-end traceability across fragmented systems, supporting compliance, operational oversight, and performance measurement without replacing legacy systems.

- **Unified agent view and basic outcome reporting (account status, PTP activity, self-service usage)**  
  *Justification:* Reduces time spent reconciling multiple systems and provides visibility into whether self-service is reducing workload and improving recovery outcomes.

---

## Out of scope

- **Hardship assessment or vulnerability detection automation**  
  *Justification:* Requires sensitive human judgment and carries high compliance and reputational risk, making it unsuitable for early automation.

- **Abusive behaviour detection and automated escalation**  
  *Justification:* High risk of false positives and incorrect handling of sensitive customer situations; requires human oversight.

- **Legal escalation workflows and enforcement actions**  
  *Justification:* Low-volume, high-risk processes that add significant complexity without contributing to Phase 1 recovery efficiency.

- **Payment processing or funds transfer functionality**  
  *Justification:* Introduces regulatory and technical complexity; Phase 1 focuses on commitments (PTP) rather than financial transactions.

- **Full replacement of the legacy collections platform**  
  *Justification:* Not feasible within Phase 1; a layered approach is required to reduce delivery and integration risk.

- **AI-driven prioritisation or predictive decisioning**  
  *Justification:* Requires mature data foundations and explainability; not necessary to achieve early operational value.

- **Bespoke repayment negotiation workflows**  
  *Justification:* Highly variable and dependent on human judgment, making it unsuitable for rules-based automation in Phase 1.

- **Advanced personalisation or recommendation engines**  
  *Justification:* Adds complexity without delivering proportional value in early release and increases delivery risk.

---

## Assumptions

- Legacy systems can provide reliable account and status data for portal display  
- Eligibility rules for PTP and routing can be agreed without full policy redesign  
- Customers can be reliably authenticated within the portal journey  
- Operations teams will continue handling complex and high-risk cases  
- A phased or pilot rollout approach is acceptable  
- Compliance requirements can be met with audit logging and restricted financial actions  

---

## Dependencies and constraints

- Integration with legacy collections and account systems  
- Agreement on PTP eligibility rules (e.g. blocked accounts, high-risk balances, frozen funds)  
- Compliance approval for identity verification, audit logging, and messaging flows  
- Alignment of agent workflows for routed cases  
- Data quality limitations across existing systems  
- Clear ownership boundaries between portal and legacy tools to avoid duplication  

---

## Why this scope is credible

This Phase 1 scope directly targets the highest-impact issues identified in discovery, particularly fragmented systems, missed follow-ups, and high volumes of repeat customer contact. By focusing on a unified account view, structured Promise-to-Pay capture, and automated follow-up tracking, it addresses both customer friction and key drivers of revenue leakage in a controlled and measurable way.

The scope is intentionally constrained to a set of high-value, low-risk capabilities that can be delivered without replacing core legacy systems. It introduces a structured self-service layer while preserving human oversight for complex and high-risk cases, ensuring operational and compliance stability.

This phased approach balances delivery feasibility with measurable early value, enabling improvements in recovery performance, operational efficiency, and customer experience.