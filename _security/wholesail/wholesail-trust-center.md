---
certifications:
- SOC 2
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Wholesail Trust Center
name_suffix: Trust Center
overview: Wholesail maintains a public trust center documenting SOC 2 and PCI DSS compliance.
provider_name: Wholesail
provider_slug: wholesail
slug: wholesail-trust-center
source_filename: wholesail-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nsource: https://www.paywholesail.com/security/\nurl: https://www.paywholesail.com/security/\n# Wholesail's own certifications are SOC 2 and PCI-DSS; ISO 27001 is inherited\n# from the Google Cloud Platform infrastructure Wholesail is hosted on.\ncertifications:\n- SOC 2\n- PCI DSS\ninherited_certifications:\n- provider: Google Cloud Platform\n  certifications: [SOC 1, SOC 2, SOC 3, PCI DSS, ISO 27001]\ncompliance_programs:\n- id: soc2\n  name: SOC 2\n  status: certified\n  scope: independent audits verifying adherence to security protocols\n- id: pci-dss\n  name: PCI DSS\n  status: compliant\n  scope: card data protection; Stripe processes/stores card details, Wholesail never sees card numbers\n- id: nacha\n  name: NACHA\n  status: compliant\n  scope: ACH money transmission (ACH processed by JP Morgan and SVB)\nsecurity_practices:\n- mandatory security training + MFA for all employees\n- device compliance monitoring\n\
  - pre-employment background checks\n- encryption at rest and TLS/HTTPS in transit\n- minimal data access + strict permission controls\n- automated logging and monitoring of payment activity\n- continuous vulnerability scanning\nfunds_protection:\n- in-transit funds held in dedicated per-merchant Stripe accounts\n- pass-through FDIC insurance up to $250,000 per customer on ACH funds\npartners: [Stripe, Plaid, Modern Treasury, JP Morgan, SVB]\nevidence:\n- source: https://www.paywholesail.com/security/\n  keywords:\n  - soc 2\n  - pci-dss\n  - nacha\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wholesail/refs/heads/main/security/wholesail-trust-center.yml
summary_line: SOC 2, PCI DSS
tags:
- Company
- Fintech
- Payments
- Accounts Receivable
- B2B
- ACH
- Wholesale
- Collections
trust_url: https://www.paywholesail.com/security/
---
