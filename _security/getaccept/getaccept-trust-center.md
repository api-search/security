---
api_specs:
- filename: getaccept-archive-api-openapi.yml
  format: yaml
  label: GetAccept Archive API
  slug: getaccept-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-archive-api-openapi.yml
- filename: getaccept-attachments-api-openapi.yml
  format: yaml
  label: GetAccept Attachments API
  slug: getaccept-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-attachments-api-openapi.yml
- filename: getaccept-authentication-api-openapi.yml
  format: yaml
  label: GetAccept Authentication API
  slug: getaccept-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-authentication-api-openapi.yml
- filename: getaccept-communication-templates-api-openapi.yml
  format: yaml
  label: GetAccept Communication Templates API
  slug: getaccept-communication-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-communication-templates-api-openapi.yml
- filename: getaccept-contacts-api-openapi.yml
  format: yaml
  label: GetAccept Contacts API
  slug: getaccept-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-contacts-api-openapi.yml
- filename: getaccept-custom-data-api-openapi.yml
  format: yaml
  label: GetAccept Custom Data API
  slug: getaccept-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-custom-data-api-openapi.yml
- filename: getaccept-documents-api-openapi.yml
  format: yaml
  label: GetAccept Documents API
  slug: getaccept-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-documents-api-openapi.yml
- filename: getaccept-others-api-openapi.yml
  format: yaml
  label: GetAccept Others API
  slug: getaccept-others-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-others-api-openapi.yml
- filename: getaccept-subscriptions-api-openapi.yml
  format: yaml
  label: GetAccept Subscriptions API
  slug: getaccept-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-subscriptions-api-openapi.yml
- filename: getaccept-templates-api-openapi.yml
  format: yaml
  label: GetAccept Templates API
  slug: getaccept-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-templates-api-openapi.yml
- filename: getaccept-users-api-openapi.yml
  format: yaml
  label: GetAccept Users API
  slug: getaccept-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-users-api-openapi.yml
- filename: getaccept-videos-api-openapi.yml
  format: yaml
  label: GetAccept Videos API
  slug: getaccept-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-videos-api-openapi.yml
certifications:
- SOC 2 Type II
- GDPR
- CCPA
- eIDAS (EU Regulation No 910/2014)
- ESIGN Act
- UETA
- Electronic Communications Act 2000
description: ''
kind: trust-center
layout: security
name: Getaccept Trust Center
name_suffix: Trust Center
overview: GetAccept maintains a public trust center documenting SOC 2 Type II, GDPR, CCPA, eIDAS (EU Regulation No 910/2014), ESIGN Act, UETA, and Electronic Communications Act 2000 compliance.
provider_name: GetAccept
provider_slug: getaccept
slug: getaccept-trust-center
source_filename: getaccept-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://www.getaccept.com/security ; https://www.getaccept.com/pricing\nurl: https://www.getaccept.com/security\ntrust_portal: false\ntrust_portal_note: >-\n  GetAccept publishes a security marketing page, not a trust center. There is no Vanta/Drata/SafeBase-style\n  portal and no self-serve document room — the SOC 2 Type II report is available on request only.\ncertifications:\n- name: SOC 2 Type II\n  status: attested\n  evidence: >-\n    \"yearly rigorous audit conducted by a reputable certified third party auditor\"; report available on\n    request\n- name: GDPR\n  status: compliant\n  evidence: stated on the security page; DPA available\n- name: CCPA\n  status: compliant\n  evidence: named on the security page\n- name: eIDAS (EU Regulation No 910/2014)\n  status: compliant\n  evidence: \"GetAccept's eSignatures are compliant with eIDAS\"\n- name: ESIGN Act\n  status: compliant\n  evidence: US electronic signature\
  \ law named on the security page\n- name: UETA\n  status: compliant\n  evidence: US electronic signature law named on the security page\n- name: Electronic Communications Act 2000\n  status: compliant\n  evidence: UK electronic signature law named on the security page\nnot_claimed:\n- ISO 27001\n- HIPAA\n- FedRAMP\n- PCI DSS\nencryption:\n  in_transit: ECDSA 256 (3072-bit-equivalent) TLS certificate\n  at_rest: AES-256\n  source: https://www.getaccept.com/security\ncontacts:\n  legal: legal@getaccept.com\n  general: hello@getaccept.com\ndocuments:\n  dpa: true\n  privacy_policy: https://www.getaccept.com/privacy-policy\n  soc2_report: on-request\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No responsible-disclosure policy, security.txt, or bug bounty (HackerOne / Bugcrowd / Intigriti) was\n    found. /.well-known/security.txt 404s on www.getaccept.com and returns the login SPA shell on the\n    app/developer hosts — see well-known/getaccept-well-known.yml. No Security\
  \ pointer is emitted.\nevidence:\n- url: https://www.getaccept.com/security\n  status: 200\n- url: https://www.getaccept.com/pricing\n  status: 200\n  note: plan page repeats GDPR / SOC 2 / eIDAS as the security posture\n- url: https://www.getaccept.com/.well-known/security.txt\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/security/getaccept-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA, eIDAS (EU Regulation No 910/2014), ESIGN Act, UETA, Electronic Communications Act 2000
tags:
- Company
- Cloud
- Sales Enablement
- Electronic Signature
- E-Signature
- Digital Sales Room
- Document Management
- Contract Management
- Proposals
- SaaS
trust_url: https://www.getaccept.com/security
---
