---
api_specs:
- filename: kufu-smarthr-openapi.json
  format: json
  label: SmartHR API
  slug: smarthr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kufu/refs/heads/main/openapi/kufu-smarthr-openapi.json
certifications:
- ISO/IEC 27001
- SOC 2
description: SmartHR's public security and compliance page, which doubles as its trust center. It names two independently attested programs — ISO/IEC 27001 (ISMS) and SOC 2 Type 2 — and lists responsible-disclosure acknowledgments. There is no third-party trust-portal product (Vanta/Drata/SafeBase); the page is first-party.
kind: trust-center
layout: security
name: Kufu Trust Center
name_suffix: Trust Center
overview: KUFU maintains a public trust center documenting ISO/IEC 27001 and SOC 2 compliance.
provider_name: KUFU
provider_slug: kufu
slug: kufu-trust-center
source_filename: kufu-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://smarthr.jp/security/\ndescription: >-\n  SmartHR's public security and compliance page, which doubles as its trust\n  center. It names two independently attested programs — ISO/IEC 27001 (ISMS)\n  and SOC 2 Type 2 — and lists responsible-disclosure acknowledgments. There is\n  no third-party trust-portal product (Vanta/Drata/SafeBase); the page is\n  first-party.\n\nurl: https://smarthr.jp/security/\nstatus: 200\nfirst_party: true\nportal_vendor: none\n\ncertifications:\n  - name: ISO/IEC 27001\n    framework: ISMS (Information Security Management System)\n    status: certified\n    certified_since: '2016-03-22'\n    scope: Information Security Management System\n    evidence: https://smarthr.jp/security/\n\n  - name: SOC 2\n    type: Type 2\n    status: report obtained\n    issuing_framework: AICPA\n    criteria:\n      - Security\n    scope: >-\n      Design and operating effectiveness of internal controls over a\
  \ defined\n      period.\n    availability: >-\n      Disclosure is restricted under SOC reporting rules; the report is\n      provided to current and prospective customers on request.\n    evidence: https://smarthr.jp/security/\n\nnot_claimed:\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - ISO/IEC 27017\n  - ISO/IEC 27018\nnote_not_claimed: >-\n  These frameworks are absent from the published page. Their absence is a real\n  finding, not an unresearched gap.\n\ngovernance:\n  board_oversight: >-\n    Internal control is overseen through regular board sessions and ISMS\n    management reviews.\n\nvulnerability_management:\n  automated_scanning: >-\n    Regular vulnerability assessment using automated tooling.\n  third_party_testing: >-\n    Annual unscheduled vulnerability assessment by external security\n    specialists.\n  disclosure: security/kufu-vulnerability-disclosure.yml\n\ncustomer_assurance:\n  security_checksheet: >-\n    A downloadable security check sheet based on METI and IPA\
  \ guidelines is\n    offered for customer due diligence.\n  tenant_controls:\n    - SSO (SAML)\n    - two-factor authentication\n    - IP address restriction\n    - audit logs\n  help_center: https://support.smarthr.jp/ja/\n\ndata_residency:\n  published: not stated on the security page\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kufu/refs/heads/main/security/kufu-trust-center.yml
summary_line: ISO/IEC 27001, SOC 2
tags:
- Company
- Human Resources
- HR Tech
- Payroll
- Employee Data
- SaaS
- Japan
- Onboarding
- Social Insurance
- Webhooks
trust_url: https://smarthr.jp/security/
---
