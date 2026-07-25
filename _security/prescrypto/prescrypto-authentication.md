---
api_key_in:
- header
api_specs:
- filename: prescrypto-hospitals-api-openapi.yml
  format: yaml
  label: Prescrypto Hospitals API
  slug: prescrypto-hospitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-hospitals-api-openapi.yml
- filename: prescrypto-locations-api-openapi.yml
  format: yaml
  label: Prescrypto Locations API
  slug: prescrypto-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-locations-api-openapi.yml
- filename: prescrypto-medics-api-openapi.yml
  format: yaml
  label: Prescrypto Medics API
  slug: prescrypto-medics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-medics-api-openapi.yml
- filename: prescrypto-memberships-api-openapi.yml
  format: yaml
  label: Prescrypto Memberships API
  slug: prescrypto-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-memberships-api-openapi.yml
- filename: prescrypto-patients-api-openapi.yml
  format: yaml
  label: Prescrypto Patients API
  slug: prescrypto-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-patients-api-openapi.yml
- filename: prescrypto-pharmacy-api-openapi.yml
  format: yaml
  label: Prescrypto Pharmacy API
  slug: prescrypto-pharmacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-pharmacy-api-openapi.yml
- filename: prescrypto-prescriptions-api-openapi.yml
  format: yaml
  label: Prescrypto Prescriptions API
  slug: prescrypto-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-prescriptions-api-openapi.yml
- filename: prescrypto-products-api-openapi.yml
  format: yaml
  label: Prescrypto Products API
  slug: prescrypto-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/openapi/prescrypto-products-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Prescrypto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prescrypto secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Prescrypto
provider_slug: prescrypto
scheme_count: 2
schemes:
- description: 'HTTP Token auth. Send: Authorization: Token <your-key>. Keys are issued by Prescrypto via direct communication and can be private (server-side) or public (browser).'
  in: header
  name: TokenAuth
  parameter: Authorization
  scheme_prefix: Token
  sources:
  - openapi/prescrypto-openapi.yml
  type: apiKey
- description: 'JWT auth for the standard-drug (products) endpoint. Send: Authorization: JWT <token>. Endpoint host (SD_ENDPOINT) and token are provisioned by Prescrypto via email.'
  in: header
  name: JWTAuth
  parameter: Authorization
  scheme_prefix: JWT
  sources:
  - openapi/prescrypto-openapi.yml
  type: apiKey
slug: prescrypto-authentication
source_filename: prescrypto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/prescrypto-openapi.yml\ndocs: https://www.prescrypto.com/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Prescrypto uses HTTP Token auth for the core integration API (Authorization: Token <key>),\n    issued through direct communication. Keys can be private (server-side) or public (browser).\n    The standard-drug (products) endpoint uses a separate JWT token (Authorization: JWT <token>)\n    on a distinct host (SD_ENDPOINT), provisioned by email. Pharmacy tokens are scoped to the\n    pharmacy endpoints only.\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_prefix: Token\n  description: 'HTTP Token auth. Send: Authorization: Token <your-key>. Keys are issued by Prescrypto\n    via direct communication and can be private (server-side) or public (browser).'\n  sources:\n  - openapi/prescrypto-openapi.yml\n- name: JWTAuth\n  type: apiKey\n\
  \  in: header\n  parameter: Authorization\n  scheme_prefix: JWT\n  description: 'JWT auth for the standard-drug (products) endpoint. Send: Authorization: JWT <token>.\n    Endpoint host (SD_ENDPOINT) and token are provisioned by Prescrypto via email.'\n  sources:\n  - openapi/prescrypto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prescrypto/refs/heads/main/authentication/prescrypto-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Healthcare
- Electronic Prescriptions
- eRx
- Pharmacy
- Telemedicine
- Medical
- Mexico
- LATAM
---
