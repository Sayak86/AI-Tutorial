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

## Notes

Use this example only for documentation or demo purposes. It is intentionally simple to highlight maintenance and adaptability issues compared to data-driven approaches.