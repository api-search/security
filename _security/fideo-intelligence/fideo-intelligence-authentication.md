---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fideo Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fideo Intelligence secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fideo Intelligence
provider_slug: fideo-intelligence
scheme_count: 1
schemes:
- applies_to:
  - POST /verify
  - POST /signals
  description: 'Authorization: Bearer {API_KEY}. A single static API key per environment. Fideo recommends separate keys per environment, key rotation, and storing keys in a secrets manager (never in client-side code).'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.fideo.ai/docs/authorization
  type: http
slug: fideo-intelligence-authentication
source_filename: fideo-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fideo.ai/docs/authorization\ndocs: https://docs.fideo.ai/docs/authorization\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    All requests to https://api.fideo.ai require a valid API key supplied as an\n    HTTP bearer token. Keys are managed inside the Fideo (ReadMe) platform or\n    issued by the Fideo support team. No OAuth2 / OpenID Connect flows and no\n    OAuth scopes are documented.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization: Bearer {API_KEY}. A single static API key per environment.\n    Fideo recommends separate keys per environment, key rotation, and storing\n    keys in a secrets manager (never in client-side code).\n  applies_to:\n  - POST /verify\n  - POST /signals\n  sources:\n  - https://docs.fideo.ai/docs/authorization\nrequired_headers:\n- name: Authorization\n  value: Bearer {API_KEY}\n\
  - name: Content-Type\n  value: application/json\nrecommended_headers:\n- name: Accept\n  value: application/json\nauth_error_codes:\n- code: 401\n  meaning: Missing or invalid API key (no account found)\n- code: 403\n  meaning: Key exists but lacks access to the requested product/endpoint\n- code: 429\n  meaning: Rate limit / trial quota exceeded\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fideo-intelligence/refs/heads/main/authentication/fideo-intelligence-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Identity
- Identity Verification
- Fraud Prevention
- Financial Crime
- KYC
- Risk Scoring
- Identity Intelligence
- Fintech
---
