---
certifications:
- SOC 2 Type II
- ISO 27001
- PCI DSS
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Liquidtrust Trust Center
name_suffix: Trust Center
overview: LiquidTrust maintains a public trust center documenting SOC 2 Type II, ISO 27001, PCI DSS, GDPR, and CCPA compliance.
provider_name: LiquidTrust
provider_slug: liquidtrust
slug: liquidtrust-trust-center
source_filename: liquidtrust-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.liquidtrust.io/security\nurl: https://trust.liquidtrust.io/\nhosted_trust_center:\n  url: https://trust.liquidtrust.io/\n  title: Liquid Trust Center\n  provider: Vanta\n  evidence: >-\n    trust.liquidtrust.io is a CNAME to cname.vantatrust.com and serves the Vanta trust-report\n    application (assets.vanta.com/static/index-trust-report.*). HTTP 200 on 2026-07-19. The report\n    body is client-rendered, so the certification list below is taken from the public security page,\n    which is the authoritative published text.\nsecurity_page: https://www.liquidtrust.io/security\ncertifications:\n- name: SOC 2 Type II\n  detail: >-\n    Audited annually, covering the security, availability, processing integrity, confidentiality, and\n    privacy trust services criteria.\n- name: ISO 27001\n  detail: Certified.\n- name: PCI DSS\n  detail: Level 1 compliant.\n- name: GDPR\n  detail: Compliant.\n- name: CCPA\n\
  \  detail: Stated compliance with CCPA and other global privacy regulations.\nencryption:\n  at_rest: AES-256, AWS KMS managed keys, automatic key rotation\n  in_transit: TLS 1.3\ncontrols:\n- 24/7 monitoring with real-time threat detection\n- Role-based access control (RBAC) and multi-factor authentication (MFA)\n- Regular penetration testing and vulnerability scanning\n- Funds held in segregated accounts at regulated U.S. financial institutions\n- AML and sanctions screening, KYB/KYC verification\nevidence:\n- source: https://www.liquidtrust.io/security\n  keywords:\n  - soc 2\n  - iso 27001\n  - pci dss\n  - gdpr\n  - ccpa\n- source: https://trust.liquidtrust.io/\n  kind: hosted trust center (Vanta)\nsee_also: conformance/liquidtrust-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidtrust/refs/heads/main/security/liquidtrust-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, PCI DSS, GDPR, CCPA
tags:
- Company
- Payments
- B2B Payments
- Escrow
- Fintech
- Cross-Border Payments
- Marketplaces
- Compliance
- KYC
- Trust and Safety
trust_url: https://trust.liquidtrust.io/
---
