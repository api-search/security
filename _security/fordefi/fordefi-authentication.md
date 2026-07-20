---
api_key_in: []
api_specs:
- filename: fordefi-openapi-original.json
  format: json
  label: Fordefi API
  slug: fordefi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fordefi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fordefi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fordefi
provider_slug: fordefi
scheme_count: 1
schemes:
- bearerFormat: JWT
  header: 'Authorization: Bearer {api_access_token}'
  name: bearerAuth
  note: API access token (JWT) issued for an API User. Sensitive/state-changing requests additionally require an ECDSA (NIST P-256) signature over "${path}|${timestamp}|${body}" sent in x-signature with x-timestamp, produced by the API Signer whose public key is registered with the API User.
  scheme: bearer
  sources:
  - openapi/fordefi-openapi-original.json
  type: http
slug: fordefi-authentication
source_filename: fordefi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fordefi-openapi-original.json\ndocs: https://docs.fordefi.com/developers/authentication\nsummary:\n  types:\n  - http\n  request_signing: ECDSA over NIST P-256 (x-signature/x-timestamp) for state-changing ops\n  transport: HTTPS only\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer {api_access_token}'\n  note: >-\n    API access token (JWT) issued for an API User. Sensitive/state-changing\n    requests additionally require an ECDSA (NIST P-256) signature over\n    \"${path}|${timestamp}|${body}\" sent in x-signature with x-timestamp, produced\n    by the API Signer whose public key is registered with the API User.\n  sources:\n  - openapi/fordefi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/authentication/fordefi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cryptocurrency
- Digital Assets
- Wallet
- Custody
- Blockchain
- DeFi
- MPC
- Payments
---
