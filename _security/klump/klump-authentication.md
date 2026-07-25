---
api_key_in:
- header
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Klump Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klump secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Klump
provider_slug: klump
scheme_count: 2
schemes:
- audience: server
  description: Every API request to the Klump endpoints must include the merchant secret key in a klump-secret-key request header. Requests with a missing, incorrect, or outdated key are rejected with 401 Unauthorized. Klump advises keeping the secret key server-side only.
  example_usage: "curl --location --request GET 'https://api.useklump.com/v1/transactions/:reference/verify' \\\n  --header 'Content-Type: application/json' \\\n  --header 'klump-secret-key: {{KLUMP_SEC_KEY}}'\n"
  in: header
  name: klump-secret-key
  parameter_name: klump-secret-key
  source: https://docs.useklump.com/docs/api-keys-authorization
  type: apiKey
- audience: client
  description: Client-side integrations pass the merchant public key as a publicKey parameter into the Klump object supplied by https://js.useklump.com/klump.js. This key is safe to expose in the browser and does not authorise server API calls.
  in: body
  key_prefix: klp_pk_
  name: publicKey
  parameter_name: publicKey
  source: https://docs.useklump.com/docs/api-keys-authorization
  type: apiKey
slug: klump-authentication
source_filename: klump-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.useklump.com/docs/api-keys-authorization\ndocs: https://docs.useklump.com/docs/api-keys-authorization\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - body\n  oauth2_flows: []\n  notes: Klump has no OAuth surface. Server-to-server calls use a merchant secret key\n    in a custom header; the browser widget is initialised with a merchant public key.\n    Keys are issued per merchant application state (TEST or LIVE) from the merchant\n    dashboard under Settings > API Keys & Webhook.\nschemes:\n- name: klump-secret-key\n  type: apiKey\n  in: header\n  parameter_name: klump-secret-key\n  audience: server\n  description: Every API request to the Klump endpoints must include the merchant secret\n    key in a klump-secret-key request header. Requests with a missing, incorrect, or\n    outdated key are rejected with 401 Unauthorized. Klump advises keeping the secret\n    key server-side only.\n  example_usage:\
  \ |\n    curl --location --request GET 'https://api.useklump.com/v1/transactions/:reference/verify' \\\n      --header 'Content-Type: application/json' \\\n      --header 'klump-secret-key: {{KLUMP_SEC_KEY}}'\n  source: https://docs.useklump.com/docs/api-keys-authorization\n- name: publicKey\n  type: apiKey\n  in: body\n  parameter_name: publicKey\n  audience: client\n  key_prefix: klp_pk_\n  description: Client-side integrations pass the merchant public key as a publicKey\n    parameter into the Klump object supplied by https://js.useklump.com/klump.js. This\n    key is safe to expose in the browser and does not authorise server API calls.\n  source: https://docs.useklump.com/docs/api-keys-authorization\nkey_management:\n  environments:\n  - name: TEST\n    description: Test keys are used while the merchant application state is set to\n      TEST in the merchant dashboard. No real money moves.\n  - name: LIVE\n    description: Live keys are used once the merchant application state is\
  \ switched\n      to LIVE and real transactions are accepted.\n  rotation: Regenerating a key immediately invalidates all previous keys; Klump will\n    not honour requests presenting a rotated key.\n  storage_guidance: Klump recommends environment variables or a key-management tool\n    (AWS Secrets Manager, HashiCorp Vault, Azure Key Vault).\n  issuance: Merchant dashboard > Settings > API Keys & Webhook\nrelated:\n  conventions: conventions/klump-conventions.yml\n  sandbox: sandbox/klump-sandbox.yml\n  errors: errors/klump-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klump/refs/heads/main/authentication/klump-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Buy Now Pay Later
- BNPL
- Fintech
- Lending
- Checkout
- E-Commerce
- Nigeria
- Africa
- Instalments
- Consumer Credit
---
