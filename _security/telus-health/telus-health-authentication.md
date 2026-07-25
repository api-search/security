---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Telus Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: TELUS Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TELUS Health
provider_slug: telus-health
scheme_count: 1
schemes:
- api: telus-health:telus-chr-enterprise-api
  bearer_format: JWT
  header: 'Authorization: Bearer {json_web_token}'
  name: chrEnterpriseJWT
  notes: No OAuth 2.0, no API keys, no SMART-on-FHIR. Partner mints a short-lived RS512 JWT signed by a private key whose public key is registered on the CHR API Consumer; access is gated behind a CHR-domain / partner agreement.
  scheme: bearer
  signing_algorithm: RS512
  token_details:
    audience: per-CHR-domain Enterprise API endpoint
    expiry: token must expire within 15 minutes (exp <= iat + 900s)
    issuer: iss claim must match the configured API Consumer
    signature: RS512 (RSA-SHA512); public key configured on the API Consumer in CHR Settings
  type: http
slug: telus-health-authentication
source_filename: telus-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://help.inputhealth.com/en/articles/6483223-making-requests-to-the-api\ndocs: https://help.inputhealth.com/en/articles/6483223-making-requests-to-the-api\nsummary:\n  types:\n  - http\n  scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: chrEnterpriseJWT\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  api: telus-health:telus-chr-enterprise-api\n  signing_algorithm: RS512\n  header: 'Authorization: Bearer {json_web_token}'\n  token_details:\n    issuer: iss claim must match the configured API Consumer\n    signature: RS512 (RSA-SHA512); public key configured on the API Consumer in CHR Settings\n    expiry: token must expire within 15 minutes (exp <= iat + 900s)\n    audience: per-CHR-domain Enterprise API endpoint\n  notes: No OAuth 2.0, no API keys, no SMART-on-FHIR. Partner mints a short-lived RS512 JWT signed by\n    a private key whose public key is registered on the\
  \ CHR API Consumer; access is gated behind a CHR-domain\n    / partner agreement.\nfhir_api:\n  api: telus-health:telus-patient-chart-fhir-api\n  scheme: none\n  note: TELUS Patient Chart is a published FHIR R4 conformance package (89 StructureDefinition profiles)\n    on Simplifier; no live authenticated TELUS FHIR endpoint is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telus-health/refs/heads/main/authentication/telus-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Canada
- EMR
- EHR
- FHIR
- HL7
- Interoperability
- GraphQL
- e-Prescribing
- Pharmacy
- Digital Health
- Clinical Data
---
