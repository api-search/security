---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Frame Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frame Payments secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Frame Payments
provider_slug: frame-payments
scheme_count: 2
schemes:
- format: 'Authorization: Bearer <secret_key>'
  key_prefixes:
    production: sk_production_
    sandbox: sk_sandbox_
  location: Authorization header
  name: SecretKey
  scheme: bearer
  type: http
  usage: Server-side. Authenticates all REST API calls. Keep out of source control, browser code, and mobile binaries.
- in: client
  key_prefixes:
    production: pk_production_
    sandbox: pk_sandbox_
  location: Frame.js initialization
  name: PublishableKey
  type: apiKey
  usage: Client-side only. Used to initialize Frame.js for card tokenization and elements; never the secret key.
slug: frame-payments-authentication
source_filename: frame-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.framepayments.com/getting-started/install\ndocs: https://docs.framepayments.com/getting-started/install\nsummary:\n  types: [apiKey]\n  scheme: bearer\n  transport: HTTPS only\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: SecretKey\n    type: http\n    scheme: bearer\n    location: Authorization header\n    format: 'Authorization: Bearer <secret_key>'\n    key_prefixes:\n      sandbox: sk_sandbox_\n      production: sk_production_\n    usage: Server-side. Authenticates all REST API calls. Keep out of source control, browser code, and mobile binaries.\n  - name: PublishableKey\n    type: apiKey\n    in: client\n    location: Frame.js initialization\n    key_prefixes:\n      sandbox: pk_sandbox_\n      production: pk_production_\n    usage: Client-side only. Used to initialize Frame.js for card tokenization and elements; never the secret key.\nenvironments:\n  toggle: Switch environments in the\
  \ Frame Dashboard at any time; test and production keys are separate.\nwebhook_auth:\n  scheme: HMAC-SHA256\n  header: X-Frame-Signature\n  format: 'sha256=<hex>'\n  secret: Per-endpoint 32-character secret generated at endpoint creation; rotate via rotateWebhookEndpointSecret.\nnotes: >-\n  Frame uses API-key (bearer secret key) authentication, not OAuth2 or OpenID\n  Connect, so there is no OAuth scope surface. Publishable keys are the\n  client-side half used by Frame.js; secret keys authenticate the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frame-payments/refs/heads/main/authentication/frame-payments-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Financial Services
- Fintech
- KYC
- Compliance
- Fraud Detection
- Billing
- Payouts
- Identity Verification
---
