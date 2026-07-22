---
api_key_in: []
api_specs:
- filename: simplifi-simplifipay-openapi.yml
  format: yaml
  label: SimpliFi Cards API
  slug: simplifi-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/openapi/simplifi-simplifipay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Simplifi Simplifipay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simplifi/Simplifipay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simplifi/Simplifipay
provider_slug: simplifi-simplifipay
scheme_count: 1
schemes:
- bearerFormat: JWT
  credentials:
  - client_id (e.g. simplifi-api-client)
  - client_secret
  - grant_type=client_credentials
  description: JWT access token obtained from POST /v1/auth/login/{companyName}.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/simplifi-simplifipay-openapi.yml
  token_endpoint: /v1/auth/login/{companyName}
  type: http
slug: simplifi-simplifipay-authentication
source_filename: simplifi-simplifipay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://apidoc.simplifipay.com/\ndocs: https://apidoc.simplifipay.com/auth.md\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: JWT\nmodel: 'Two-legged login: exchange client_id + client_secret (grant_type=client_credentials) at POST /v1/auth/login/{companyName}\n  for a JWT access token, then send it as Authorization: Bearer <token> on every subsequent call. A separate\n  SDK-admin token (POST /v1/auth/sdk/{companyName}) is minted for the Virtual Card SDK. Every request\n  also requires a unique requestUuid header (20-40 chars) for traceability.'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token obtained from POST /v1/auth/login/{companyName}.\n  token_endpoint: /v1/auth/login/{companyName}\n  credentials:\n  - client_id (e.g. simplifi-api-client)\n  - client_secret\n  - grant_type=client_credentials\n  sources:\n  - openapi/simplifi-simplifipay-openapi.yml\n\
  credentials_provisioning: Sandbox credentials (client_id/client_secret and companyName) are issued after\n  registering at https://simplifipay.com/contact-us/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplifi-simplifipay/refs/heads/main/authentication/simplifi-simplifipay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cards
- Card Issuing
- Virtual Cards
- Fintech
- Payments
- Banking as a Service
- Embedded Finance
- GCC
- Webhooks
---
