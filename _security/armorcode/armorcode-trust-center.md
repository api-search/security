---
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Armorcode Trust Center
name_suffix: Trust Center
overview: ArmorCode maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: ArmorCode
provider_slug: armorcode
slug: armorcode-trust-center
source_filename: armorcode-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.armorcode.com/security\nprobe: true\nurl: https://www.armorcode.com/security\ncertifications:\n- SOC 2 Type 2\nsummary: >-\n  ArmorCode publishes its security posture on the /security page rather than a\n  standalone trust portal. The vanity host trust.armorcode.com 301-redirects to\n  the marketing homepage (no dedicated trust center). The /security page states\n  ArmorCode has attained SOC 2 Type 2 compliance and attestation, and documents\n  256-bit SSL/TLS encryption (ECDHE_RSA key exchange), tenant isolation with\n  separate data partitions, and key-management systems.\nevidence:\n- source: https://www.armorcode.com/security\n  keywords: [soc 2 type 2, compliance, attestation, tenant isolation, encryption]\nnotes:\n- trust.armorcode.com returns HTTP 301 -> https://www.armorcode.com/ (no standalone trust center)\n- Only SOC 2 Type 2 is named; no public ISO 27001 / PCI DSS / HIPAA / FedRAMP / GDPR claim on this\
  \ page\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armorcode/refs/heads/main/security/armorcode-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Security
- Application Security
- Vulnerability Management
- ASPM
- Exposure Management
- DevSecOps
- Compliance
- API
trust_url: https://www.armorcode.com/security
---
