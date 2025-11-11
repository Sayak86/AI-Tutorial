# AI-Tutorial

This repository contains small examples and demonstrations related to AI techniques.

## Example: rule-based transaction filters

Below is a simple rule-based snippet (for demonstration only):

```
IF income > 100,000 CHF AND debt_ratio < 0.3 THEN approve
IF payment_destination IN sanctioned_countries THEN block
IF transaction_time BETWEEN 02:00 AND 05:00 THEN flag_for_review
```

## Limitations of this rule-based approach

- Brittle: rules break when new patterns or variations appear (e.g., new sanctioned destinations, changed timestamp formats, or noisy data).
- Hard to maintain: every new fraud pattern requires manual rule changes and deployment.
- Limited expressiveness: rules capture simple, linear logic but miss complex correlations across multiple features or long-term behavior.
- Poor at generalization: rules tend to overfit known cases and miss novel attacks.
- Latency and scale: large rule sets become slow and error-prone to evaluate in high-throughput systems.

This snippet is included to demonstrate the limitations of purely rule-based systems for fraud detection and risk decisions. For production systems, consider complementary approaches such as behavior-based anomaly detection, statistical models, supervised ML classifiers, or hybrid rule+ML systems that can adapt to changing patterns.

---

## Age 2: Machine Learning (2000s-2020)

Computer learns patterns from data

### Swiss Banking Example: Credit Scoring with ML

- **Training:** Feed model 100,000 past credit decisions
- **Learning:** Model discovers hidden patterns
- **Result:** Predicts approval likelihood for new applications

### The Breakthrough

- ✅ Finds patterns humans miss
- ✅ Adapts automatically to new data
- ✅ Handles 200+ variables simultaneously
- ✅ Improves with more examples

### Discovered Pattern Example

> "Customers who pay utility bills 3+ days early have 40% lower default rates" — something no human analyst specified, but ML discovered from data.

---

## Age 3: Generative AI (2022-Present)

AI creates new content, not just analyzes

### Swiss Banking Example: Automated Documentation

**Input:** Transaction data + compliance requirements

**Output:**
- Complete suspicious activity report (SAR) narrative
- Loan rejection letter with explanations
- Customer service responses in 4 languages

### The Magic

- ✨ Doesn't just classify (fraud/not fraud)
- ✨ Creates explanations, documents, code, analyses
- ✨ Understands context and nuance
- ✨ Communicates in natural language

---

## Transition Statement

> "Each age built on the previous. Rules gave us control. ML gave us adaptability. GenAI gave us communication. Now in 2025, we're entering **Age 4: Agentic AI** — systems that don't just answer, they act."

### Speaker Notes

Use the credit scoring example throughout — it's something everyone understands. Show the progression: manual rules → learned patterns → generated content. This sets up the "why 2022 mattered" story in Category 3.

---

## Notes

Use this example only for documentation or demo purposes. It is intentionally simple to highlight maintenance and adaptability issues compared to data-driven approaches.