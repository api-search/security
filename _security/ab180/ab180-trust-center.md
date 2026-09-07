---
api_specs:
- filename: overview
  format: yaml
  label: Airbridge API
  slug: airbridge-api
  spec_type: Postman
  url: https://www.postman.com/airbridge-engineering/workspace/airbridge-api/overview
certification_count: 5
certifications:
- SOC 2 Type 2
- ISO/IEC 27001
- ISO/IEC 27017
- ISO/IEC 27018
- ISMS (KISA)
description: ''
kind: trust-center
layout: security
name: Ab180 Trust Center
name_suffix: Trust Center
overview: Ab180 maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, and ISMS (KISA) compliance.
provider_name: Ab180
provider_slug: ab180
slug: ab180-trust-center
source_filename: ab180-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nprobe: true\nurl: https://www.airbridge.io/en/information-security\nhttp_status: 200\nchecked: '2026-09-05'\nnote: 'Airbridge serves no trust.airbridge.io or security.airbridge.io host — trust.airbridge.io\n  resolves to the marketing site root. The information-security page is the trust surface,\n  and it names auditors and certificate identifiers rather than only claiming compliance.'\ncertifications:\n- name: SOC 2 Type 2\n  auditor: Deloitte Anjin LLC\n  statement: 'Successfully completed the SOC 2 Type 2 examination in accordance with AICPA\n    and IAASB attestation standards.'\n- name: ISO/IEC 27001\n  version: '2013'\n  certifier: SGS\n- name: ISO/IEC 27017\n  version: '2015'\n  certifier: SGS\n- name: ISO/IEC 27018\n  version: '2019'\n  certifier: SGS\n- name: ISMS (KISA)\n  certificate_id: ISMS-KISA-2023-138\n  certifier: Korea Internet & Security Agency\n  statement: Certified after a rigorous audit of 80 items.\nprivacy_regimes:\n\
  - GDPR\n- CCPA\n- PIPL\ninfrastructure:\n  cloud: AWS\n  primary_region: Tokyo (ap-northeast-1)\n  data_residency: 'Airbridge advertises data residency options for regional data processing\n    requirements, and announced an AWS Seoul region service for Korean regulatory and\n    security requirements.'\n  residency_source: https://www.airbridge.io/ko/blog/seoul-region-launch-data-compliance\nencryption:\n  in_transit: TLS 1.2 or higher\n  at_rest: AWS SSE-S3 (AES-256) for sensitive data\n  passwords: PBKDF2\ntesting:\n  internal: 'Product penetration testing in accordance with the SDLC, plus regular internal\n    penetration tests.'\n  third_party: Annual third-party testing.\n  customer_testing_policy: 'Customers must not perform penetration testing or security\n    vulnerability checks against the Airbridge system without approval from the AB180\n    Security & Privacy Team.'\nvulnerability_disclosure:\n  published: false\n  note: 'No security.txt on any host, no bug bounty program\
  \ (HackerOne / Bugcrowd /\n    Intigriti), and no security@ address or disclosure form is published. The page names an\n    \"AB180 Security & Privacy Team\" but gives no reporting channel. NO VulnerabilityDisclosure\n    or Security pointer is emitted for this provider, because the surface a researcher would\n    need does not exist.'\nevidence:\n- source: https://www.airbridge.io/en/information-security\n  keywords: [soc 2, iso 27001, iso 27017, iso 27018, isms, encryption, penetration testing]\n  http_status: 200\n- source: https://www.airbridge.io/en/solutions/security-privacy\n  keywords: [gdpr, ccpa, pipl, data residency, skan]\n  http_status: 200\n- source: https://trust.airbridge.io/\n  result: 'Redirects to https://www.airbridge.io/en — no dedicated trust host.'\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ab180/refs/heads/main/security/ab180-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISMS (KISA)
tags:
- Company
- Attribution
- Mobile Measurement
- Marketing
- Analytics
- Advertising
- Deep Linking
- Mobile
- Reporting
- South Korea
trust_url: https://www.airbridge.io/en/information-security
---
