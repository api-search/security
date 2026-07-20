---
api_key_in: []
auth_types:
- http
description: Every request to the Fideo Verify and Signals API (https://api.fideo.ai) authenticates with a bearer API key supplied in the HTTP Authorization header. Keys are managed inside the ReadMe-hosted developer hub (Settings -> API Keys) or issued by the Fideo support team for dedicated test/production credentials. There is no OAuth2 / OpenID Connect flow and no per-request signing; the static key is scoped per workspace and inherits the account's contracted rate limits.
kind: authentication
layout: security
method: searched
name: Fideo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fideo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fideo
provider_slug: fideo
scheme_count: 1
schemes:
- description: 'Authorization: Bearer {API_KEY} — required on every Verify and Signals request. Keys are provisioned/rotated in ReadMe; separate keys per environment (prod/staging) and per workflow are recommended. Never embed keys in client-side code; proxy calls through a backend you control.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.fideo.ai/docs/authorization
  type: http
slug: fideo-authentication
source_filename: fideo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fideo.ai/docs/authorization\ndocs: https://docs.fideo.ai/docs/authorization\ndescription: >-\n  Every request to the Fideo Verify and Signals API (https://api.fideo.ai)\n  authenticates with a bearer API key supplied in the HTTP Authorization header.\n  Keys are managed inside the ReadMe-hosted developer hub (Settings -> API Keys)\n  or issued by the Fideo support team for dedicated test/production credentials.\n  There is no OAuth2 / OpenID Connect flow and no per-request signing; the static\n  key is scoped per workspace and inherits the account's contracted rate limits.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization: Bearer {API_KEY} — required on every Verify and Signals\n    request. Keys are provisioned/rotated in ReadMe; separate keys per\n    environment (prod/staging)\
  \ and per workflow are recommended. Never embed\n    keys in client-side code; proxy calls through a backend you control.\n  sources:\n  - https://docs.fideo.ai/docs/authorization\nrequired_headers:\n- header: Authorization\n  value: Bearer {API_KEY}\n  required: true\n- header: Content-Type\n  value: application/json\n  required: true\n- header: Accept\n  value: application/json\n  required: false\nauth_errors:\n- status: 401\n  meaning: Missing or invalid/revoked API key.\n- status: 403\n  meaning: Key exists but is not entitled for the requested product (Verify or Signals).\nkey_management:\n- Create separate keys per environment (prod vs staging) and per workflow/service.\n- Never embed keys in client-side code; originate calls from a secure backend.\n- Rotate regularly; keep two active keys per environment for zero-downtime rotation.\n- Store keys in a secret manager (Vault, AWS Secrets Manager) and inject via env vars.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fideo/refs/heads/main/authentication/fideo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Identity Verification
- Fraud Prevention
- Fraud Detection
- Identity Intelligence
- KYC
- AML
- Financial Crime
- Compliance
- Fintech
- Sanctions Screening
- Risk Scoring
---
