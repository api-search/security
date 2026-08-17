---
certifications:
- ISO 27001:2013
- SAS 70 / SOC 2
- ISO 27001:2013
- SAS 70 / SSAE 16
- PCI DSS
- GDPR
description: ''
kind: trust-center
layout: security
name: Revv Trust Center
name_suffix: Trust Center
overview: Revv maintains a public trust center documenting ISO 27001:2013, SAS 70 / SOC 2, ISO 27001:2013, SAS 70 / SSAE 16, PCI DSS, and GDPR compliance.
provider_name: Revv
provider_slug: revv
slug: revv-trust-center
source_filename: revv-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://www.revv.so/trust/security.html\nurl: https://www.revv.so/trust/security.html\ntitle: Revv Trust Center — Security & privacy center\nnote: >-\n  The automated probe (probe-security-programs.py) missed this page because it lives at\n  /trust/security.html rather than trust.<domain> or /trust; it was found by reading the\n  site navigation and confirmed by fetch (HTTP 200, 2026-08-14). Read the certification\n  list carefully: most of the named certifications belong to Revv's SUPPLIERS, not to\n  Revv. The page states AWS data centres are ISO 27001:2013 / SAS 70-SSAE 16 / PCI DSS\n  certified and GDPR compliant, that payment card handling is Stripe's PCI DSS scope, and\n  that eSignature legal compliance is delivered \"in partnership with OneSpan\". Of Revv's\n  OWN posture the page says only that Revv \"is building its system to be compliant with\n  ISO 27001:2013 and SAS 70 (SOC 2) standards with the certification\
  \ work under review\".\n  That directly contradicts the product pricing page, which claims \"SOC2 Compliance — our\n  app and infrastructure is SOC2 certified\"; the discrepancy is recorded, not resolved.\ncertifications:\n- name: ISO 27001:2013\n  holder: Revv\n  status: in-progress\n  claim: '\"building its system to be compliant ... with the certification work under review\"'\n- name: SAS 70 / SOC 2\n  holder: Revv\n  status: disputed\n  claim: >-\n    trust/security.html says \"under review\"; pricing.html says \"our app and\n    infrastructure is SOC2 certified\"\n- name: ISO 27001:2013\n  holder: Amazon Web Services (hosting provider)\n  status: inherited\n- name: SAS 70 / SSAE 16\n  holder: Amazon Web Services (hosting provider)\n  status: inherited\n- name: PCI DSS\n  holder: Stripe (payment processor) / AWS\n  status: inherited\n  claim: Revv does not process credit card information; Stripe handles payments\n- name: GDPR\n  holder: Amazon Web Services (hosting provider)\n  status:\
  \ inherited\nregulatory_compliance:\n- ESIGN Act (US)\n- UETA (US)\n- eIDAS / Regulation 910/2014/EC (EU)\n- Information Technology Act 2000 (India)\nesignature_partner: OneSpan Sign\nsecurity_practices:\n- Data at rest encrypted in AWS RDS via AWS KMS (FIPS 140-2 validated HSMs)\n- S3 server-side encryption (SSE-S3)\n- AWS CloudTrail key-usage logging\n- Periodic internal infosec/compliance audit on a 6-month cadence\n- Security policy review with remediation steps\ncontacts:\n  security: security@revvsales.com\n  support: support@revv.so\nrelated:\n  privacy_policy: https://www.revv.so/privacy.html\n  terms_of_use: https://www.revv.so/termsofuse.html\n  data_processing_agreement: https://www.revv.so/data-processing-agreement.html\nx-evidence:\n- url: https://www.revv.so/trust/security.html\n  status: 200\n  fetched: '2026-08-14'\n  keywords:\n  - trust center\n  - compliance\n  - iso 27001\n  - soc 2\n  - pci dss\n  - gdpr\n  - encryption\n- url: https://www.revv.so/pricing.html\n  status:\
  \ 200\n  fetched: '2026-08-14'\n  keywords:\n  - soc2 compliance\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revv/refs/heads/main/security/revv-trust-center.yml
summary_line: ISO 27001:2013, SAS 70 / SOC 2, ISO 27001:2013, SAS 70 / SSAE 16, PCI DSS, GDPR
tags:
- Company
- Document Automation
- Electronic Signature
- Contract Management
- Sales Enablement
- Workflow Automation
- SaaS
trust_url: https://www.revv.so/trust/security.html
---
