---
api_specs:
- filename: surfe-account-api-openapi.yml
  format: yaml
  label: Surfe Account API
  slug: surfe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-account-api-openapi.yml
- filename: surfe-companies-api-openapi.yml
  format: yaml
  label: Surfe Companies API
  slug: surfe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-companies-api-openapi.yml
- filename: surfe-people-api-openapi.yml
  format: yaml
  label: Surfe People API
  slug: surfe-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-people-api-openapi.yml
- filename: surfe-recommendations-api-openapi.yml
  format: yaml
  label: Surfe Recommendations API
  slug: surfe-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-recommendations-api-openapi.yml
certifications:
- ISO 27001
- GDPR
description: Surfe publishes a public security page rather than a hosted trust centre. There is no trust.surfe.com (DNS does not resolve) and no third-party trust portal (Vanta / Drata / SafeBase / Whistic) was found. The page names two postures — ISO/IEC 27001 certification and GDPR compliance as both processor and controller — and describes encryption, access and incident-response practices in prose. No certification report, audit letter, or evidence download is offered, and SOC 2 is not claimed.
kind: trust-center
layout: security
name: Surfe Trust Center
name_suffix: Trust Center
overview: Surfe maintains a public trust center documenting ISO 27001 and GDPR compliance.
provider_name: Surfe
provider_slug: surfe
slug: surfe-trust-center
source_filename: surfe-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.surfe.com/security/\ndescription: >-\n  Surfe publishes a public security page rather than a hosted trust centre.\n  There is no trust.surfe.com (DNS does not resolve) and no third-party trust\n  portal (Vanta / Drata / SafeBase / Whistic) was found. The page names two\n  postures — ISO/IEC 27001 certification and GDPR compliance as both processor\n  and controller — and describes encryption, access and incident-response\n  practices in prose. No certification report, audit letter, or evidence\n  download is offered, and SOC 2 is not claimed.\ncertifications:\n- name: ISO 27001\n  claimed: true\n  scope_statement: >-\n    \"Our ISO27001 certification sets rigorous requirements for managing and\n    protecting sensitive data.\"\n  auditor: not disclosed\n  certificate_available: false\n- name: GDPR\n  claimed: true\n  role: both Data Processor and Data Controller\n  certificate_available: false\n  note:\
  \ GDPR is a regulation, not a certification; recorded as a stated compliance posture.\nnot_claimed:\n- SOC 2\n- ISO 27017\n- ISO 27018\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\nstated_controls:\n- CRM data accessed on demand only, over secured API connections, never without consent.\n- Data never sold under any circumstances.\n- Encryption in transit and at rest, including encrypted databases and secure OAuth token storage.\n- Salesforce OAuth used for user authentication so credentials are not entered into Surfe.\n- Disaster and incident-response plans maintained, tested and audited annually.\n- Data backed up (\"Data rescue\").\nrelated_pages:\n- {name: Security, url: 'https://www.surfe.com/security/', status: 200}\n- {name: Privacy Policy, url: 'https://www.surfe.com/privacy-policy/', status: 200}\n- {name: Data Protection, url: 'https://www.surfe.com/data-protection/', status: 200}\n- {name: Terms and Conditions, url: 'https://www.surfe.com/terms-and-conditions/', status: 200}\n\
  - {name: Terms and Conditions – API, url: 'https://www.surfe.com/terms-and-conditions-api/', status: 200}\n- {name: Legitimate Interests Assessment, url: 'https://www.surfe.com/legitimate-interests-assessment/'}\n- {name: Opt-out Mechanism, url: 'https://www.surfe.com/opt-out-mechanism/'}\n- {name: Legal Notice, url: 'https://www.surfe.com/legal-notice/'}\n- {name: Cookie Policy, url: 'https://www.surfe.com/cookie-policy/'}\ndata_protection_note: >-\n  Surfe sells B2B contact data, so its GDPR posture carries unusual weight for\n  buyers: it publishes a Legitimate Interests Assessment and a data-subject\n  opt-out mechanism as separate public pages, which is more than most providers\n  in this category expose.\nevidence:\n- source: https://www.surfe.com/security/\n  http_status: 200\n  fetched: '2026-08-13'\n  keywords: [iso 27001, iso27001 certified, gdpr compliant, encryption, incident response, data processor, data controller]\n- source: https://www.surfe.com/pricing/\n  http_status:\
  \ 200\n  fetched: '2026-08-13'\n  quote: Surfe is ISO27001 certified and GDPR compliant.\nprobed_absent:\n- {url: 'https://trust.surfe.com/', result: 'DNS did not resolve (curl exit 6, status 000)'}\n- {url: 'https://www.surfe.com/trust/', status: 404}\n- {url: 'https://www.surfe.com/security-and-compliance/', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/security/surfe-trust-center.yml
summary_line: ISO 27001, GDPR
tags:
- B2B Data
- Contact Data
- Sales Intelligence
- Enrichment
- Lead Generation
- CRM
- Prospecting
trust_url: https://www.surfe.com/security/
---
