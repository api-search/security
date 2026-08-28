---
certifications:
- SOC 2 Type 2
- SOC 3
- ISO 27001:2013
- ISO 9001:2015
- TX-RAMP
description: ''
kind: trust-center
layout: security
name: Safe Security Trust Center
name_suffix: Trust Center
overview: SAFE Security maintains a public trust center documenting SOC 2 Type 2, SOC 3, ISO 27001:2013, ISO 9001:2015, and TX-RAMP compliance.
provider_name: SAFE Security
provider_slug: safe-security
slug: safe-security-trust-center
source_filename: safe-security-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://safe.security/security/\nname: SAFE Security trust center\nurl: https://safe.security/security/\nhttp_status: 200\ndedicated_trust_portal: false\nnote: >-\n  SAFE has no trust portal in the Vanta/Drata/SafeBase sense - trust.safe.security does not\n  resolve (DNS NXDOMAIN) and there is no evidence-request or NDA-gated document exchange.\n  What exists is a single public Security Statement page on the marketing site, plus one\n  downloadable report. It is unusually substantive for a marketing page and it names the\n  certifications explicitly, but the artefacts behind them are not published apart from the\n  SOC 3.\ncertifications:\n- name: SOC 2 Type 2\n  public_report: false\n- name: SOC 3\n  public_report: true\n  url: https://safe.security/wp-content/uploads/safe-security-soc3-report-2026.pdf\n  http_status: 200\n  content_type: application/pdf\n  note: Downloadable with no form, no login and no NDA - the strongest\
  \ single piece of published assurance evidence SAFE offers.\n- name: ISO 27001:2013\n  public_report: false\n- name: ISO 9001:2015\n  public_report: false\n- name: TX-RAMP\n  public_report: false\n  note: The Texas state cloud authorization programme, not federal FedRAMP.\nsecurity_controls:\n  hosting: AWS, customer-selected region at tenant signup\n  data_residency_doc: https://docs.safe.security/docs/data-residency-in-safe\n  encryption_in_transit: TLS 1.2 over public networks\n  encryption_at_rest: AES-256 via AWS KMS\n  customer_managed_keys: true\n  cmk_note: Customers may supply their own AWS KMS key, in which case key generation and management access sit entirely with the customer.\n  byoa: true\n  byoa_note: >-\n    \"Bring Your Own Account\" customers run SAFE in their own AWS account and get\n    CloudWatch and CloudTrail log access for SIEM ingestion.\n  tenancy: per-tenant, per-region\nobserved_posture:\n  source: security/safe-security-domain-security.yml\n  tls: TLSv1.3\
  \ negotiated on safe.security, docs.safe.security and us.safeone.ai\n  hsts: enabled on all three hosts\n  dnssec:\n    safe.security: true\n    safeone.ai: false\n  caa: none published on either domain\n  spf: present on both domains\n  dmarc: present on both domains, policy quarantine\n  note: >-\n    Worth reading against the certifications: safeone.ai - the domain the PRODUCT and both\n    APIs are served from - has no DNSSEC, neither domain publishes CAA records, and both\n    DMARC policies stop at quarantine rather than reject. These are exactly the outside-in\n    controls SAFE's own TPRM product assesses third parties on.\nevidence:\n- url: https://safe.security/security/\n  status: 200\n- url: https://safe.security/wp-content/uploads/safe-security-soc3-report-2026.pdf\n  status: 200\n- url: https://trust.safe.security/\n  status: null\n  note: DNS does not resolve\ngaps_for_provider:\n- No trust portal; certifications are prose rather than requestable artefacts.\n- No FedRAMP,\
  \ HIPAA or PCI DSS attestation published despite healthcare and financial verticals being marketed.\n- No subprocessor list published.\n- CAA records absent on both domains; DNSSEC absent on safeone.ai.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safe-security/refs/heads/main/security/safe-security-trust-center.yml
summary_line: SOC 2 Type 2, SOC 3, ISO 27001:2013, ISO 9001:2015, TX-RAMP
tags:
- Company
- Security
- Cyber Risk Quantification
- Third-Party Risk Management
- Continuous Threat Exposure Management
- AI Security Posture Management
- Risk Management
- Governance Risk and Compliance
- FAIR
- Vulnerability Management
trust_url: https://safe.security/security/
---
