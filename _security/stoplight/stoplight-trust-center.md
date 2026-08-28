---
api_specs:
- filename: stoplight-platform-v1-openapi.yml
  format: yaml
  label: Stoplight v1 Platform API
  slug: stoplight-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stoplight/refs/heads/main/openapi/stoplight-platform-v1-openapi.yml
certifications:
- SOC 2
- ISO/IEC 27001
- NIST CSF
description: Trust and compliance posture covering Stoplight. Stoplight publishes no trust center of its own; since the 2023 SmartBear acquisition its compliance program is the parent's, published at trust.smartbear.com and summarised on smartbear.com/security.
kind: trust-center
layout: security
name: Stoplight Trust Center
name_suffix: Trust Center
overview: Stoplight maintains a public trust center documenting SOC 2, ISO/IEC 27001, and NIST CSF compliance.
provider_name: Stoplight
provider_slug: stoplight
slug: stoplight-trust-center
source_filename: stoplight-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://smartbear.com/security/ and https://trust.smartbear.com/\nprovider: Stoplight\nproviderId: stoplight\ndescription: >-\n  Trust and compliance posture covering Stoplight. Stoplight publishes no trust\n  center of its own; since the 2023 SmartBear acquisition its compliance program is\n  the parent's, published at trust.smartbear.com and summarised on smartbear.com/security.\ntrust_center:\n  url: https://trust.smartbear.com/\n  status: 200\n  probed: '2026-08-27'\n  operator: SmartBear\n  platform: SafeBase\n  note: >-\n    The trust center itself is a client-rendered SafeBase application; the named\n    certifications below were read from the server-rendered SmartBear security page,\n    not from the SafeBase shell.\nsummary_page:\n  url: https://smartbear.com/security/\n  status: 200\n  probed: '2026-08-27'\ncertifications:\n  - name: SOC 2\n    scope: Service Organization Control\n    source: https://smartbear.com/security/\n\
  \    evidence_type: named-on-vendor-page\n  - name: ISO/IEC 27001\n    scope: Information Security Management\n    source: https://smartbear.com/security/\n    evidence_type: named-on-vendor-page\n  - name: NIST CSF\n    scope: Cybersecurity Framework alignment\n    source: https://smartbear.com/security/\n    evidence_type: named-on-vendor-page\nprivacy_regimes:\n  - name: GDPR\n    source: https://smartbear.com/security/\n  - name: CCPA\n    source: https://smartbear.com/security/\npractices_published:\n  - Secure design and architecture reviews\n  - Code scanning and dependency analysis\n  - Vulnerability management and remediation\n  - Controlled change management processes\n  - Monitoring, detection and incident response\nstoplight_specific:\n  url: https://stoplight.io/security-practices\n  status: 200\n  probed: '2026-08-27'\n  note: >-\n    Stoplight's own product security-practices page, still served on the Stoplight\n    domain and still the most product-specific security document\
  \ available.\ncaveat: >-\n  Certification artifacts (audit reports, certificates) are behind the SafeBase\n  request flow. Nothing here asserts a report was inspected — only that SmartBear\n  publicly names these certifications for the estate that includes Stoplight.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stoplight/refs/heads/main/security/stoplight-trust-center.yml
summary_line: SOC 2, ISO/IEC 27001, NIST CSF
tags:
- API Design
- API Documentation
- API Governance
- AsyncAPI
- Design-First
- Linting
- Mock Servers
- OpenAPI
- SmartBear API Hub
- Style Guides
trust_url: ''
---
