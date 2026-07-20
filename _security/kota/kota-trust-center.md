---
api_specs:
- filename: kota-openapi-original.json
  format: json
  label: Kota API
  slug: kota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kota/refs/heads/main/openapi/kota-openapi-original.json
certifications:
- SOC 2
- ISO 27001
- HIPAA
- GDPR
description: Kota runs a hosted Trust Centre at trust.kota.io carrying full policies, ISO audit reports and real-time controls monitoring, backed by a detailed public security page. Certifications held by Kota itself are distinguished below from those inherited from its cloud hosting providers.
kind: trust-center
layout: security
name: Kota Trust Center
name_suffix: Trust Center
overview: Kota maintains a public trust center documenting SOC 2, ISO 27001, HIPAA, and GDPR compliance.
provider_name: Kota
provider_slug: kota
slug: kota-trust-center
source_filename: kota-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.kota.io/security, https://trust.kota.io/\nurl: https://trust.kota.io/\nsecurity_page: https://www.kota.io/security\ndescription: >-\n  Kota runs a hosted Trust Centre at trust.kota.io carrying full policies, ISO audit reports and\n  real-time controls monitoring, backed by a detailed public security page. Certifications held by\n  Kota itself are distinguished below from those inherited from its cloud hosting providers.\ncertifications:\n- SOC 2\n- ISO 27001\n- HIPAA\n- GDPR\ncertification_detail:\n- name: ISO 27001:2022\n  held_by: Kota\n  status: audit completed\n- name: GDPR\n  held_by: Kota\n  status: compliance committed; assists customers with their obligations\n- name: PCI DSS\n  held_by: Stripe (payment processor)\n  status: card processing delegated to Stripe at PCI Level 1; Kota stores no card data\n- name: SOC 1\n  held_by: Microsoft Azure (hosting)\n  status: inherited from infrastructure\
  \ provider\n- name: SOC 2\n  held_by: Microsoft Azure (hosting)\n  status: inherited from infrastructure provider\n- name: SOC 3\n  held_by: Microsoft Azure (hosting)\n  status: inherited from infrastructure provider\n- name: HIPAA\n  held_by: Microsoft Azure (hosting)\n  status: supported by infrastructure provider\nhosting:\n  regions: EU\n  providers:\n  - Microsoft Azure\n  - Google Cloud Platform\nsecurity_controls:\n  encryption_at_rest: AES256, with additional at-work encryption in the database\n  encryption_in_transit: 256-bit SSL / TLS 1.3, using both ECDSA and RSA algorithms\n  https_enforced: true\n  security_headers:\n  - X-Frame-Options\n  - X-XSS-Protection\n  - Content-Security-Policy\n  backups: daily automated backups, full redundancy and disaster recovery\n  access_control: employee access to customer data strictly limited and audited\n  logging: detailed log collection for incident investigation\n  vulnerability_management: automated vulnerability monitoring across all\
  \ code; continuous updates\n  mfa: RFC 6238-compatible authenticator app 2FA (shipped v4.2.6, 2026-04-08)\nevidence:\n- source: https://www.kota.io/security\n  keywords:\n  - soc 2\n  - iso 27001\n  - hipaa\n  - trust center\n  - trust centre\n  - gdpr\n- source: https://trust.kota.io/\n  keywords:\n  - trust center\nrelated:\n  vulnerability_disclosure: security/kota-vulnerability-disclosure.yml\n  conformance: conformance/kota-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kota/refs/heads/main/security/kota-trust-center.yml
summary_line: SOC 2, ISO 27001, HIPAA, GDPR
tags:
- Company
- Fintech
- Insurance
- Employee Benefits
- Health Insurance
- Pensions
- Insurtech
- Embedded Finance
- Human Resources
- Payroll
trust_url: https://trust.kota.io/
---
