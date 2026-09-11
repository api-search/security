---
api_specs:
- filename: fraud-net-public-apis-openapi.json
  format: json
  label: Fraud.net Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/openapi/fraud-net-public-apis-openapi.json
certification_count: 7
certifications:
- SOC 2 Type II
- ISO 27001
- PCI DSS
- HIPAA
- GDPR
- NIST 800-53
- NTIS
description: ''
kind: trust-center
layout: security
name: Fraud Net Trust Center
name_suffix: Trust Center
overview: Fraud.net maintains a public trust center documenting SOC 2 Type II, ISO 27001, PCI DSS, HIPAA, GDPR, NIST 800-53, and NTIS compliance.
provider_name: Fraud.net
provider_slug: fraud-net
slug: fraud-net-trust-center
source_filename: fraud-net-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nprobe: true\nsource: https://www.fraud.net/trust-center\nurl: https://www.fraud.net/trust-center\nprovider: Fraud.net\nproviderId: fraud-net\ncertifications:\n  - SOC 2 Type II\n  - ISO 27001\n  - PCI DSS\n  - HIPAA\n  - GDPR\n  - NIST 800-53\n  - NTIS\ndocuments:\n  - {name: 'PCI - DSS', access: request, label: 'Get Access'}\n  - {name: SOC2 Type II Attestation Report, access: request, label: 'Get Access'}\ncontrol_families:\n  - Access Control (Zero Trust, MFA, RBAC, least privilege, segregation of duties, MDM)\n  - Awareness & Training (induction + annual, role-specific, secure-coding workshops)\n  - Audit and Accountability (centralized read-only log platform, anomaly monitoring, time sync)\n  - Assessment, Authorization and Monitoring (internal + independent audits, annual penetration testing, continuous vulnerability scanning)\n  - Configuration Management (change management, baselines, peer-reviewed build, IDS)\n  - Contingency\
  \ Planning (RTO/RPO, daily backups, annual restoration test, quarterly DR test)\n  - Identification and Authentication (SSO/AD, mandatory MFA, NIST 800-63B passwords)\n  - Security Incident Response (IR plans, cross-functional teams, post-incident review)\n  - Maintenance / Media Protection (AWS sanitization + encryption, BYOD policy)\n  - Planning / Personnel Security (regulatory monitoring, background checks, de-provisioning)\n  - Risk Assessment / Secure SDLC / Supply Chain Risk Management\n  - System and Communications Protection (encryption at rest and in transit, TLS 1.2+)\nstatements:\n  encryption: >-\n    \"Customer data is encrypted at rest and in transit using industry-standard methods\n    (e.g., TLS 1.2+).\"\n  hosting: '\"We are a 100% cloud-born service provider\"; AWS named as the infrastructure provider.'\nevidence:\n  - source: https://www.fraud.net/trust-center\n    http_status: 200\n    fetched: '2026-09-10'\n    keywords: [trust center, soc 2, iso27001, pci dss, hipaa,\
  \ gdpr, nist 800-53, penetration testing]\nsecurity_contact: null\nvulnerability_disclosure: null\nnote: >-\n  The Trust Center is a real, substantive, public compliance page — it names seven\n  frameworks and publishes a control narrative — but it carries NO security contact\n  address and NO responsible-disclosure or bug-bounty channel. The mechanical\n  probe-security-programs.py pass returned trust=none because it looks at\n  trust.<domain>/security.<domain>/<domain>/trust and this page is at /trust-center;\n  this file is the searched upgrade, with the fetched status recorded.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/security/fraud-net-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, PCI DSS, HIPAA, GDPR, NIST 800-53, NTIS
tags:
- Fraud
- Risk
- Commerce
- Payments
- Security
- Compliance
- Identity
- Banking
- Machine Learning
trust_url: https://www.fraud.net/trust-center
---
