---
api_specs:
- filename: aeropay-v2-openapi.yml
  format: yaml
  label: Aeropay v2 API
  slug: aeropay-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/openapi/aeropay-v2-openapi.yml
certification_count: 2
certifications:
- SOC 2
- Nacha ACH Operating Rules
description: ''
kind: trust-center
layout: security
name: Aeropay Trust Center
name_suffix: Trust Center
overview: Aeropay maintains a public trust center documenting SOC 2 and Nacha ACH Operating Rules compliance.
provider_name: Aeropay
provider_slug: aeropay
slug: aeropay-trust-center
source_filename: aeropay-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: https://www.aeropay.com/trust-center\nurl: https://www.aeropay.com/trust-center\npublished: true\ncertifications:\n- name: SOC 2\n  status: compliant\n  cadence: annual independent audit\n  scope: security, availability and confidentiality controls\n  report_available: false\n  report_type_published: false\n  quote: 'Aeropay is SOC 2 compliant, with annual independent audits verifying that our security,\n    availability, and confidentiality controls meet enterprise-grade standards.'\n- name: Nacha ACH Operating Rules\n  status: compliant\n  cadence: annual independent audit of ACH processes\n  scope: ACH operations\n  quote: 'We handle ACH operations in strict compliance with NACHA standards, and undergo annual\n    independent audits of our ACH processes.'\npractices_claimed:\n- OAuth-first bank linking through the Aerosync widget\n- FDX-style normalization of bank data\nnot_claimed:\n- PCI DSS\n- ISO/IEC 27001\n- HIPAA\n\
  - FedRAMP\n- GDPR certification\nthird_party_trust_portal:\n  present: false\n  note: 'No Vanta, Drata, SafeBase or Conveyor trust portal is linked; the trust center is a marketing page\n    on the Webflow site, not a document exchange. No SOC 2 report, penetration-test summary, subprocessor\n    list or security questionnaire is downloadable, and there is no gated request form for one.'\nvulnerability_disclosure:\n  present: false\n  note: 'The trust center names no vulnerability disclosure policy, responsible disclosure process, bug\n    bounty program or security contact address. No /.well-known/security.txt is served on any Aeropay host\n    (well-known/aeropay-well-known.yml). probe-security-programs.py returned vdp=none. A researcher who\n    finds a flaw in a live payments network has no published channel to report it. NO type: Security\n    pointer is emitted in apis.yml because no disclosure program exists to point at.'\njurisdiction:\n  countries:\n  - US\n  note: Aeropay states\
  \ it currently supports U.S. bank accounts only.\nlegal:\n  privacy_policy: https://www.aeropay.com/legal/privacy-policy\n  terms_merchant: https://www.aeropay.com/legal/terms-of-service\n  terms_end_user: https://www.aeropay.com/legal/terms-of-service---end-user\nevidence:\n- url: https://www.aeropay.com/trust-center\n  status: 200\n- url: https://www.aeropay.com/.well-known/security.txt\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeropay/refs/heads/main/security/aeropay-trust-center.yml
summary_line: SOC 2, Nacha ACH Operating Rules
tags:
- Payments
- Pay by bank
- ACH
- Open Banking
- Fintech
- Bank linking
- Financial Services
- Real-time payments
- Webhook
- Payouts
- MCP
- Risk & fraud
trust_url: https://www.aeropay.com/trust-center
---
