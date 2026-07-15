---
certifications:
- PCI DSS
- SOC 2
- ISO 27001
- GDPR
description: Checkout.com's security & compliance posture, captured from its PCI compliance documentation. Checkout Technology Ltd (a company within the Checkout.com group) is certified as a PCI DSS Level 1 Service Provider — the highest standard set by the payment card industry. Integrating via Flow, Hosted Payments Page, Payment Links, or the Mobile SDKs lets merchants accept payments without ever handling card data, simplifying their own PCI scope (typically SAQ A). This is the human-verified searched fill; the automated trust-center probe did not record it because Checkout.com surfaces compliance through its docs rather than a trust.<domain> subdomain meeting the probe's keyword threshold.
kind: trust-center
layout: security
name: Checkout Com Trust Center
name_suffix: Trust Center
overview: Checkout.com maintains a public trust center documenting PCI DSS, SOC 2, ISO 27001, and GDPR compliance.
provider_name: Checkout.com
provider_slug: checkout-com
slug: checkout-com-trust-center
source_filename: checkout-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nprobe: false\nsource: https://www.checkout.com/docs/payments/ensure-regulatory-compliance/pci-compliance\nurl: https://www.checkout.com/docs/payments/ensure-regulatory-compliance/pci-compliance\ndescription: >-\n  Checkout.com's security & compliance posture, captured from its PCI compliance\n  documentation. Checkout Technology Ltd (a company within the Checkout.com\n  group) is certified as a PCI DSS Level 1 Service Provider — the highest\n  standard set by the payment card industry. Integrating via Flow, Hosted\n  Payments Page, Payment Links, or the Mobile SDKs lets merchants accept payments\n  without ever handling card data, simplifying their own PCI scope (typically\n  SAQ A). This is the human-verified searched fill; the automated trust-center\n  probe did not record it because Checkout.com surfaces compliance through its\n  docs rather than a trust.<domain> subdomain meeting the probe's keyword\n  threshold.\ncertifications:\n\
  \  - {name: PCI DSS, level: Service Provider Level 1, entity: Checkout Technology Ltd, note: Highest standard set by the payment card industry.}\n  - {name: SOC 2, note: Reported by third-party security profiles; details provided to customers on request.}\n  - {name: ISO 27001, note: Information security management certification reported for the Checkout.com group.}\n  - {name: GDPR, scope: EU/UK data protection compliance.}\nmerchant_scope_reduction:\n  note: >-\n    Merchants simplify their own PCI compliance by integrating with Flow, Hosted\n    Payments Page, Payment Links, or Mobile SDKs (no card data handled), serving\n    all payment pages over TLS/HTTPS, and validating annually (most via SAQ A).\ndocs:\n  - https://www.checkout.com/docs/payments/ensure-regulatory-compliance/pci-compliance\n  - https://www.checkout.com/docs/payments/ensure-regulatory-compliance/sca-compliance\nevidence:\n  - {source: https://www.checkout.com/docs/payments/ensure-regulatory-compliance/pci-compliance,\
  \ keywords: [pci dss level 1, service provider, self-assessment questionnaire, tls]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/security/checkout-com-trust-center.yml
summary_line: PCI DSS, SOC 2, ISO 27001, GDPR
tags:
- Fintech
- Payments
- Cards
- Acquiring
- Cross-Border
trust_url: https://www.checkout.com/docs/payments/ensure-regulatory-compliance/pci-compliance
---
