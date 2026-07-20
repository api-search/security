---
api_key_in: []
api_specs:
- filename: kanastra-banking-openapi.yml
  format: yaml
  label: Kanastra Banking API
  slug: kanastra-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanastra/refs/heads/main/openapi/kanastra-banking-openapi.yml
auth_types:
- http
- private_key_jwt
description: ''
kind: authentication
layout: security
method: searched
name: Kanastra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kanastra secures its APIs with http and private_key_jwt across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kanastra
provider_slug: kanastra
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer JWT access token obtained from POST /api/v1/auth/token. Token response includes tokenType=Bearer, expiresIn (~35999s / ~10h), and a space-delimited scope claim.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kanastra-banking-openapi.yml
  type: http
slug: kanastra-authentication
source_filename: kanastra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# generated: '2026-07-19'\ngenerated: '2026-07-19'\nmethod: searched\nsource: https://banking-docs.kanastra.com.br/\ndocs: https://banking-docs.kanastra.com.br/\nsummary:\n  types:\n  - http\n  - private_key_jwt\n  token_endpoint: /api/v1/auth/token\n  registration_endpoint: /api/v1/auth/jwks\n  assertion_alg: ES512\n  bearer_ttl_seconds: 35999\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer JWT access token obtained from POST /api/v1/auth/token. Token response includes\n    tokenType=Bearer, expiresIn (~35999s / ~10h), and a space-delimited scope claim.\n  sources:\n  - openapi/kanastra-banking-openapi.yml\nflow:\n  style: private_key_jwt (client assertion)\n  steps:\n  - Register an ES512 (secp521r1) public key for your clientId via POST /api/v1/auth/jwks. Private key\n    stays with the integrator.\n  - Build and sign a JWT client assertion (clientAssertion) with the ES512 private key.\n  - POST /api/v1/auth/token\
  \ with {clientId, clientAssertion} to receive a Bearer access_token + scope.\n  - 'Send Authorization: Bearer <access_token> on all subsequent calls.'\nadditional_controls:\n- name: Transaction Hash Key\n  algorithm: HMAC-SHA256 (hex-encoded)\n  applies_to:\n  - POST /api/v1/accounts/personal\n  description: Account-creation endpoints require an HMAC-SHA256 hash of the request payload (shared secret\n    provided by Kanastra at onboarding), hex-encoded and passed in request headers.\n- name: PIX OTP\n  description: PIX key registration approval/denial is confirmed with an OTP token (Approve/Deny/Resend\n    OTP endpoints under PIX Keys).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanastra/refs/heads/main/authentication/kanastra-authentication.yml
summary_line: http/private_key_jwt · 1 scheme
tags:
- Company
- Banking
- Banking as a Service
- Payments
- PIX
- Boleto
- Private Credit
- Fintech
- Brazil
- Wealth Management
---
