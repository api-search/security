---
api_specs:
- filename: canopy-openapi.json
  format: json
  label: Canopy Connect API
  slug: canopy-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/openapi/canopy-openapi.json
certification_count: 1
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Canopy Trust Center
name_suffix: Trust Center
overview: Canopy Connect maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Canopy Connect
provider_slug: canopy
slug: canopy-trust-center
source_filename: canopy-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://www.usecanopy.com/company/is-canopy-connect-safe\nprovider: Canopy Connect\nproviderId: canopy\ntrust_portal: null\ntrust_portal_note: >-\n  No trust center portal. trust.usecanopy.com does not resolve (NXDOMAIN,\n  probed 2026-09-05) and no Vanta/Drata/SafeBase/Whistic-style portal is linked\n  from the site. Compliance is asserted in marketing prose on two public pages.\npages:\n  - url: https://www.usecanopy.com/company/is-canopy-connect-safe\n    title: Is Canopy Connect Safe?\n    status: 200\n  - url: https://www.usecanopy.com/security\n    title: Security\n    status: 200\n  - url: https://www.usecanopy.com/resources/permissioned-data\n    title: Permissioned data\ncertifications:\n  - name: SOC 2 Type 2\n    claimed: true\n    quote: We are SOC II Type 2 Certified, following strict information security policies and procedures.\n    source: https://www.usecanopy.com/company/is-canopy-connect-safe\n    report_available:\
  \ false\n    auditor: null\n    audit_period: null\n    note: >-\n      Asserted in prose only. No report, no auditor name, no audit window, and\n      no NDA-gated request flow is published.\ncontrols:\n  - name: Encryption at rest\n    value: 256-bit AES\n    source: https://www.usecanopy.com/company/is-canopy-connect-safe\n  - name: Encryption in transit\n    value: TLS 1.3+\n    source: https://www.usecanopy.com/company/is-canopy-connect-safe\n  - name: SSL Labs grade\n    value: A+ (claimed)\n    source: https://www.usecanopy.com/company/is-canopy-connect-safe\n  - name: Infrastructure\n    value: Amazon Web Services\n    source: https://www.usecanopy.com/company/is-canopy-connect-safe\n  - name: Credential handling\n    value: >-\n      Canopy Connect states it never shares consumer login and password\n      information with any third party. Canopy Connect Components tokenizes\n      carrier credentials in the browser so they never reach the integrator's\n      server.\n    source:\
  \ https://docs.usecanopy.com/reference/components-getting-started\nnot_claimed:\n  - ISO 27001\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - GDPR certification\n  - CCPA attestation\n  - GLBA\n  - FCRA\ngaps:\n  - No subprocessor list published.\n  - No data-retention schedule published (custom retention is sold as an Enterprise tier feature).\n  - No penetration-test summary or vulnerability-management statement.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/security/canopy-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Auto Insurance
- Casualty
- Financial-Services
- Homeowners Insurance
- Insurance
- Insurance Verification
- Property
trust_url: ''
---
