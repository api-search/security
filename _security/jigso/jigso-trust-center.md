---
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Jigso Trust Center
name_suffix: Trust Center
overview: Jigso maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Jigso
provider_slug: jigso
slug: jigso-trust-center
source_filename: jigso-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.jigso.io/security-portal\nurl: https://www.jigso.io/security-portal\n# Only certifications/programs Jigso itself claims. The probe's keyword match\n# additionally caught ISO 27001, PCI DSS, HIPAA and FedRAMP, but the /security\n# page attributes those to AWS (the infrastructure provider), NOT to Jigso -\n# removed to avoid asserting certifications Jigso does not hold.\ncertifications:\n- SOC 2 Type II\n- GDPR\nprograms:\n- name: SOC 2 Type II\n  status: certified\n  scope: security, availability, confidentiality, and privacy\n- name: GDPR\n  status: readiness program implemented\nnotes: >-\n  Jigso encrypts customer data at rest and in transit, supports customer-managed\n  encryption keys (BYOK), and states annual penetration testing by CREST-accredited\n  vendors. A Security Addendum and privacy documentation are published on the\n  security portal. No formal public vulnerability-disclosure policy\
  \ was found.\nevidence:\n- source: https://www.jigso.io/security-portal\n  keywords:\n  - soc 2 type ii\n  - gdpr\n  - encryption at rest and in transit\n- source: https://www.jigso.io/security\n  keywords:\n  - soc2 compliance\n  - gdpr readiness program\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jigso/refs/heads/main/security/jigso-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- Artificial Intelligence
- Enterprise
- Business Intelligence
- Revenue Operations
- Model Context Protocol
- Agents
- Data Integration
- Customer Success
- Sales
trust_url: https://www.jigso.io/security-portal
---
