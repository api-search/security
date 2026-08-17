---
certifications:
- SOC 2 Type II
- HIPAA
- PCI DSS
- GDPR
- CSA CAIQ
description: ''
kind: trust-center
layout: security
name: Symblai Trust Center
name_suffix: Trust Center
overview: Symbl.ai maintains a public trust center documenting SOC 2 Type II, HIPAA, PCI DSS, GDPR, and CSA CAIQ compliance.
provider_name: Symbl.ai
provider_slug: symblai
slug: symblai-trust-center
source_filename: symblai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://symbl.ai/platform/security/overview/\ndocs: https://symbl.ai/platform/security/overview/\nnotes: >-\n  Symbl.ai publishes a public \"Security, Privacy and Compliance\" page naming five specific\n  attestations/programs. It is a marketing-hosted security overview, not a hosted trust portal:\n  there is no evidence room, no self-service report download, no subprocessor list and no\n  document request flow, and trust.symbl.ai does not resolve. Certification names and the\n  encryption claims below are quoted from the page; API Evangelist has NOT verified any\n  attestation with the auditor or the certifying body.\ntype: security-overview-page\nhosted_portal: false\nportal_probes:\n- url: https://trust.symbl.ai/\n  result: NXDOMAIN\n- url: https://symbl.ai/platform/security/overview/\n  http_status: 200\ncertifications:\n- name: SOC 2 Type II\n  claimed: true\n  scope: Product, infrastructure and policies, assessed by an\
  \ independent third-party auditor.\n  report_available: false\n  report_note: No self-service report download or NDA request flow is published.\n- name: HIPAA\n  claimed: true\n  scope: >-\n    Offers HIPAA Business Associate Agreements to healthcare customers, and signs Business\n    Associate Contracts as required.\n  report_available: false\n- name: PCI DSS\n  claimed: true\n  scope: Compliant with the Payment Card Industry Data Security Standard.\n  report_available: false\n- name: GDPR\n  claimed: true\n  scope: >-\n    New vendors, assets and personal-data processing activities are subject to privacy,\n    security and compliance review; documented process for personal-data transfers out of the\n    EU/UK.\n  report_available: false\n- name: CSA CAIQ\n  claimed: true\n  scope: >-\n    Completed the Cloud Security Alliance Consensus Assessments Initiative Questionnaire\n    security assessment.\n  report_available: false\n  registry_verified: false\n  registry_note: Not verified against\
  \ the CSA STAR registry by API Evangelist.\nsecurity_program:\n  data_security:\n    tls_minimum_claimed: TLS 1.2\n    in_transit: RSA 2048-bit keys; connections secured with 2048-bit encryption.\n    at_rest: AES-256.\n  product_security: >-\n    States a secure-by-design developer process covering development, deployment and post-\n    deployment, with a software delivery and change-management model.\n  risk_management: >-\n    States a flexible risk-management framework for identification, assessment, treatment and\n    reporting of security risks, plus identity and access management controls.\nprivacy_policy: https://symbl.ai/privacy-policy/\nterms_of_service: https://symbl.ai/termsofservice/\nsubprocessors_published: false\ncaveat: >-\n  These claims describe a platform whose API, console and documentation hosts no longer resolve\n  (see lifecycle/symblai-lifecycle.yml). The page is live and current-facing as published;\n  whether the attestations remain in force under Invoca ownership\
  \ is not stated anywhere public.\nx-evidence:\n  fetched: '2026-08-14'\n  url: https://symbl.ai/platform/security/overview/\n  http_status: 200\n  content_type: text/html; charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symblai/refs/heads/main/security/symblai-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, PCI DSS, GDPR, CSA CAIQ
tags:
- Company
- Conversation Intelligence
- Speech to Text
- Voice AI
- Artificial Intelligence
- Machine Learning
- Real Time
- SDKs
trust_url: ''
---
