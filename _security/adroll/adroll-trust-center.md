---
certifications:
- SOC 2
- SOC 3
- ISO 27001
- PCI DSS
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Adroll Trust Center
name_suffix: Trust Center
overview: AdRoll maintains a public trust center documenting SOC 2, SOC 3, ISO 27001, PCI DSS, GDPR, and CCPA compliance.
provider_name: AdRoll
provider_slug: adroll
slug: adroll-trust-center
source_filename: adroll-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://security.nextroll.com/\nplatform: SafeBase\nparent_page: https://www.nextroll.com/trust-center\nnote: >-\n  NextRoll runs a real, populated SafeBase trust portal for AdRoll and AdRoll\n  ABM. The automated probe in probe-security-programs.py missed it because it\n  checks trust.<domain> and <domain>/trust — NextRoll uses security.nextroll.com,\n  linked from https://www.nextroll.com/trust-center. Reports themselves are\n  request-gated behind SafeBase's NDA flow; the certification inventory below is\n  what the portal states publicly.\n\ncertifications:\n- name: SOC 2\n  detail: SOC 2 Type 2 Report\n  auditor: Sensiba\n  document_available: on request via SafeBase\n- name: SOC 3\n  detail: SOC 3 Report\n  auditor: Sensiba\n- name: ISO 27001\n  detail: ISO 27001 - 2013\n- name: PCI DSS\n  auditor: Security Metrics\n- name: GDPR\n- name: CCPA\n\nassessments:\n- {name: CAIQ v4.0.2, kind: self-assessment}\n- {name:\
  \ SIG Lite, kind: self-assessment}\n- {name: VSA Full, kind: self-assessment}\n- {name: Pentest Report, auditor: HackerOne}\n\nsecurity_ratings_published:\n- BitSight\n- Black Kite\n- CyberVadis\n- ImmuniWeb\n- RiskRecon\n- SecurityScorecard\n- UpGuard\n- Qualys SSL Labs\n- MDN Observatory\n- CryptCheck\n- CIS Score\n\nprogram_areas_documented:\n- Access Control\n- App Security\n- Audit Logging\n- BC/DR\n- Change Management\n- Code Analysis\n- Corporate Security\n- Data Security (encryption at rest and in transit, disk encryption, data classification)\n- Endpoint Security (EDR, MDM)\n- Incident Response\n- Infrastructure (AWS, VPC, WAF, anti-DDoS, IDS/IPS, separate production environment, zero trust)\n- Network Security\n- Physical Security\n- Product Security\n- Risk Management\n- Software Development Lifecycle\n- Subprocessors\n- Vulnerability & Patch Management\n- AI\n\npolicies_listed:\n- Acceptable Use Policy\n- Access Control Policy\n- Backup Policy\n- Data Classification Policy\n\
  - Encryption Policy\n- Incident Response Policy\n- Information Security Policy\n- Physical Security Policy\n- Risk Assessment/Management Policy\n- Software Development Lifecycle Policy\n\nprivacy:\n  privacy_portal: https://nextroll-privacy.relyance.ai/\n  dpo_contact: dpo@nextroll.com\n  gdpr_page: https://www.nextroll.com/trust-center/gdpr\n  privacy_policy: https://www.nextroll.com/privacy\n  your_privacy_choices: https://www.nextroll.com/your-privacy-choices\n\nevidence:\n- source: https://security.nextroll.com/\n  http_status: 200\n  keywords: [SOC 2, SOC 3, ISO 27001, PCI DSS, GDPR, CCPA, Pentest Report, Responsible Disclosure, SafeBase]\n- source: https://www.nextroll.com/trust-center\n  http_status: 200\n  keywords: [Trust Center, Security portal, GDPR, CCPA]\n\nx-evidence:\n  checked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adroll/refs/heads/main/security/adroll-trust-center.yml
summary_line: SOC 2, SOC 3, ISO 27001, PCI DSS, GDPR, CCPA
tags:
- Advertising
- Display Advertising
- Retargeting
- Marketing
- AdTech
- Programmatic
trust_url: https://security.nextroll.com/
---
