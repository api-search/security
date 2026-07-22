---
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Vesence Trust Center
name_suffix: Trust Center
overview: Vesence maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Vesence
provider_slug: vesence
slug: vesence-trust-center
source_filename: vesence-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.vesence.com/security\nname: Vesence Trust & Security\nurl: https://www.vesence.com/security\nsummary: >-\n  Vesence publishes a security page describing independent audits, encryption,\n  tenant isolation, and compliance posture for professional-services firms\n  handling sensitive legal and financial work inside Microsoft Office.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  detail: Independently audited controls for security, availability, and confidentiality.\n- name: GDPR\n  status: compliant\n  detail: GDPR compliant with all processing in the European Union.\ncontrols:\n  data_protection:\n  - Never trains AI models on customer data\n  - Content Filtering and Abuse Monitoring turned off at the Azure level (not even Microsoft can access data)\n  - Documents processed in memory and never persisted beyond the session\n  - All customer data logically isolated per tenant (Zero Data Retention)\n\
  \  encryption:\n  - TLS 1.3 in transit\n  - AES-256 at rest\n  - Data encrypted within a secure Azure private environment\n  infrastructure:\n  - Hosted on Microsoft Azure European Central region\n  - Zero Trust architecture; every request verified regardless of origin\n  - 24/7 automated monitoring and threat detection\n  - Redundant architecture with automatic failover and point-in-time recovery\n  authentication:\n  - Microsoft Entra ID integration with token-based authentication\n  - SAML & SSO through the customer identity provider\n  - Role-Based Access Control (RBAC) with least-privilege principles\n  - Multi-factor authentication enforced for all accounts\n  - Comprehensive audit logging and automated session management\n  compliance:\n  - GDPR compliant with all processing in the European Union\n  - SOC 2 Type II certified, aligned with industry standards\n  - Regular third-party security audits and vulnerability assessments\n  - Incident response plan with defined SLAs\nsubprocessors_page:\
  \ https://www.vesence.com/subprocessors\ncontact: hello@vesence.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesence/refs/heads/main/security/vesence-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- Ai
- Agentic AI
- Legal Tech
- Professional Services
- Microsoft Office
- Document Automation
trust_url: https://www.vesence.com/security
---
