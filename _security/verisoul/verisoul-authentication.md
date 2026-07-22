---
api_key_in:
- header
api_specs:
- filename: verisoul-session-openapi.json
  format: json
  label: Verisoul Session API
  slug: verisoul-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-session-openapi.json
- filename: verisoul-account-openapi.json
  format: json
  label: Verisoul Account API
  slug: verisoul-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-account-openapi.json
- filename: verisoul-list-openapi.json
  format: json
  label: Verisoul Lists API
  slug: verisoul-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-list-openapi.json
- filename: verisoul-phone-openapi.json
  format: json
  label: Verisoul Phone API
  slug: verisoul-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-phone-openapi.json
- filename: verisoul-email-openapi.json
  format: json
  label: Verisoul Email Intelligence API
  slug: verisoul-email-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-email-openapi.json
- filename: verisoul-email-batch-openapi.json
  format: json
  label: Verisoul Email Intelligence Batch API
  slug: verisoul-email-intelligence-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-email-batch-openapi.json
- filename: verisoul-idcheck-openapi.json
  format: json
  label: Verisoul ID Check API
  slug: verisoul-id-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-idcheck-openapi.json
- filename: verisoul-facematch-openapi.json
  format: json
  label: Verisoul Face Match API
  slug: verisoul-face-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-facematch-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Verisoul Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verisoul secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Verisoul
provider_slug: verisoul
scheme_count: 2
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/verisoul-session-openapi.json
  - openapi/verisoul-account-openapi.json
  - openapi/verisoul-list-openapi.json
  - openapi/verisoul-phone-openapi.json
  - openapi/verisoul-email-openapi.json
  - openapi/verisoul-email-batch-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/verisoul-facematch-openapi.json
  - openapi/verisoul-idcheck-openapi.json
  type: apiKey
slug: verisoul-authentication
source_filename: verisoul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/*-openapi.json + https://docs.verisoul.ai/api-reference/introduction\ndocs: https://docs.verisoul.ai/api-reference/introduction\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Every Verisoul API endpoint is authenticated with a secret API key sent in\n    the `x-api-key` request header. Keys are environment-scoped: separate keys\n    for Production (api.prod.verisoul.ai) and Sandbox (api.sandbox.verisoul.ai),\n    issued per project from the dashboard. There is no OAuth 2.0 or OIDC surface.\n    Frontend/mobile SDKs authenticate with a public Project ID (not the secret\n    API key); the secret key must never be exposed in client-side code.\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    sources:\n      - openapi/verisoul-session-openapi.json\n      - openapi/verisoul-account-openapi.json\n      - openapi/verisoul-list-openapi.json\n\
  \      - openapi/verisoul-phone-openapi.json\n      - openapi/verisoul-email-openapi.json\n      - openapi/verisoul-email-batch-openapi.json\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    sources:\n      - openapi/verisoul-facematch-openapi.json\n      - openapi/verisoul-idcheck-openapi.json\nkey_management:\n  issuer: https://dashboard.verisoul.ai/developers\n  environments:\n    - {name: production, base_url: https://api.prod.verisoul.ai}\n    - {name: sandbox, base_url: https://api.sandbox.verisoul.ai}\n  project_id_note: >-\n    Frontend SDKs (Web/iOS/Android/React Native/Flutter) are initialized with a\n    public Project ID; the x-api-key secret is backend-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/authentication/verisoul-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Fraud Detection
- Identity Verification
- Fake Account Detection
- Device Fingerprinting
- Email Intelligence
- Bot Detection
- KYC
- Trust and Safety
- Risk Scoring
---
