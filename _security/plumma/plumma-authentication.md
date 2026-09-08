---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: plumma-connect-openapi.yml
  format: yaml
  label: Plumma CONNECT API
  slug: plumma-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plumma/refs/heads/main/openapi/plumma-connect-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Plumma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plumma secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plumma
provider_slug: plumma
scheme_count: 1
schemes:
- description: Your X.509 client certificate, base64-encoded.
  in: header
  name: ApiKeyAuth
  parameter: x-plumma-connect-api-key
  sources:
  - openapi/plumma-connect-openapi.yml
  type: apiKey
slug: plumma-authentication
source_filename: plumma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/plumma-connect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-plumma-connect-api-key\n  description: Your X.509 client certificate, base64-encoded.\n  sources:\n  - openapi/plumma-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plumma/refs/heads/main/authentication/plumma-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Telecommunications
- Network APIs
- Italy
- Europe
- GSMA Open Gateway
- CAMARA
- API Aggregator
- Fraud Prevention
- Identity Verification
- SIM Swap
- KYC
- Age Verification
- Number Verification
- Telco Intelligence
- Software Development
---
