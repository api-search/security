---
api_specs:
- filename: unqork-customer-api-openapi.yml
  format: yaml
  label: Unqork Customer API
  slug: unqork-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/openapi/unqork-customer-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2013
- HIPAA
- FedRAMP
- GDPR
description: Unqork runs a hosted Trust Center at trust.unqork.com (Vanta), and publishes a human-readable security & compliance overview at unqork.com/security-compliance plus a platform governance page at unqork.com/security-governance. The Trust Center itself is a client-rendered single-page application, so the certification list below was read from the public security-compliance page rather than from the Vanta document index (which requires JS execution / a request for access).
kind: trust-center
layout: security
name: Unqork Trust Center
name_suffix: Trust Center
overview: Unqork maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2013, HIPAA, FedRAMP, and GDPR compliance.
provider_name: Unqork
provider_slug: unqork
slug: unqork-trust-center
source_filename: unqork-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nprobe: true\nurl: https://trust.unqork.com/\nplatform: Vanta Trust Center\ndescription: >-\n  Unqork runs a hosted Trust Center at trust.unqork.com (Vanta), and publishes a\n  human-readable security & compliance overview at unqork.com/security-compliance\n  plus a platform governance page at unqork.com/security-governance. The Trust\n  Center itself is a client-rendered single-page application, so the certification\n  list below was read from the public security-compliance page rather than from\n  the Vanta document index (which requires JS execution / a request for access).\npages:\n  - url: https://trust.unqork.com/\n    title: unqork.com Trust Center\n    kind: trust-center\n    http_status: 200\n    rendering: client-side (Vanta SPA)\n  - url: https://unqork.com/security-compliance/\n    title: Security & Compliance\n    kind: compliance-overview\n    http_status: 200\n  - url: https://unqork.com/security-governance/\n    title:\
  \ Security & Governance\n    kind: platform-governance\n    http_status: 200\ncertifications:\n  - name: SOC 2 Type II\n    detail: >-\n      Unqork undergoes annual SOC 2 Type II examinations with AICPA-certified\n      third-party auditors; controls are tested to verify control effectiveness.\n  - name: ISO/IEC 27001:2013\n    detail: Unqork states it is ISO/IEC 27001:2013 certified.\n  - name: HIPAA\n    detail: >-\n      Listed as an industry-mandated standard Unqork maintains security\n      compliance with.\n  - name: FedRAMP\n    detail: >-\n      Unqork states it is live in the FedRAMP Marketplace; supporting controls\n      include FIPS-validated cryptography and PIV/CAC authentication for US\n      Government customers.\n  - name: GDPR\n    detail: >-\n      Unqork processes client data as a processor under the General Data\n      Protection Regulation.\nsecurity_practices:\n  encryption: AES-256 at rest, FIPS-validated cryptography suites in transit and at rest\n  authentication:\
  \ PIV/CAC authentication supported for US Government customers\n  penetration_testing: >-\n    Third-party penetration testing performed at least annually, plus\n    continuous automated scanning, static analysis and dynamic application\n    security testing prior to application go-live.\n  vulnerability_management: >-\n    Continuous platform-level monitoring with automated per-application\n    oversight including daily static scans.\n  audit_trail: >-\n    Platform-level change tracking of what changed, when, and by whom, across\n    the application lifecycle.\nrelated:\n  disclosure: security/unqork-vulnerability-disclosure.yml\n  domain_security: security/unqork-domain-security.yml\n  conformance: conformance/unqork-conformance.yml\nevidence:\n  - source: https://trust.unqork.com/\n    fetched: '2026-07-31'\n    http_status: 200\n    keywords: [trust center, security, compliance]\n  - source: https://unqork.com/security-compliance/\n    fetched: '2026-07-31'\n    http_status: 200\n\
  \    keywords: [soc 2 type ii, iso/iec 27001, hipaa, fedramp, gdpr, fips]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/security/unqork-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2013, HIPAA, FedRAMP, GDPR
tags:
- Company
- No-Code
- Low-Code
- Application Development
- Enterprise Software
- Platform as a Service
- Workflow
- Financial Services
- Insurance
- Government
- Application Modernization
trust_url: https://trust.unqork.com/
---
