---
api_key_in:
- header
api_specs:
- filename: coinme-caas-openapi.json
  format: json
  label: Coinme Crypto-as-a-Service API
  slug: coinme-crypto-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinme/refs/heads/main/openapi/coinme-caas-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Coinme Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coinme secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coinme
provider_slug: coinme
scheme_count: 2
schemes:
- description: HTTP Basic on POST /authorize — partnerId as username, clientsecret as password. Exchanged for a 60-minute JWT authorization token.
  docs: https://docs.coinme.com/docs/get-authorization
  name: basic
  scheme: basic
  sources:
  - openapi/coinme-caas-openapi.json
  type: http
- description: Partner API key passed in the x-api-key header on CaaS operations (e.g. quotes, transactions).
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/coinme-caas-openapi.json
  type: apiKey
slug: coinme-authentication
source_filename: coinme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/coinme-caas-openapi.json\ndocs: https://docs.coinme.com/docs/get-authorization\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: partner-credential\n  flow: >-\n    Two-step. (1) Partner obtains credentials from Coinme (partnerId, clientsecret, User-Agent).\n    (2) POST /authorize with HTTP Basic (partnerId=username, clientsecret=password) and the\n    partner User-Agent header to obtain a JWT authorization token. The token is cached and passed\n    as the Authorization bearer on every subsequent CaaS call; some endpoints also require an\n    x-api-key header. Token TTL is 60 minutes in production, 30 minutes in staging.\n  consumer_oauth:\n    note: >-\n      Separate from the partner CaaS API, Coinme consumer accounts authenticate via an OIDC provider\n      at auth.coinme.com (grants: authorization_code, refresh_token, client_credentials,\n      token-exchange, device_code; scopes: openid,\
  \ profile, email). See scopes/coinme-scopes.yml.\n    issuer: https://auth.coinme.com\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic on POST /authorize — partnerId as username, clientsecret as password. Exchanged for\n    a 60-minute JWT authorization token.\n  docs: https://docs.coinme.com/docs/get-authorization\n  sources:\n  - openapi/coinme-caas-openapi.json\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Partner API key passed in the x-api-key header on CaaS operations (e.g. quotes, transactions).\n  sources:\n  - openapi/coinme-caas-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinme/refs/heads/main/authentication/coinme-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto
- Cryptocurrency
- Payments
- Bitcoin
- Wallet
- KYC
- Onboarding
- Fintech
- Crypto-as-a-Service
- On-Ramp
- Off-Ramp
---
