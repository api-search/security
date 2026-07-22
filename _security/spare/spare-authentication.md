---
api_key_in:
- header
api_specs:
- filename: spare-bahrain-authentication-openapi-original.json
  format: json
  label: Spare Bahrain Authentication API
  slug: spare-bahrain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-bahrain-authentication-openapi-original.json
- filename: spare-bahrain-ais-openapi-original.json
  format: json
  label: Spare Bahrain Account Information API
  slug: spare-bahrain-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-bahrain-ais-openapi-original.json
- filename: spare-bahrain-pis-openapi-original.json
  format: json
  label: Spare Bahrain Payment Initiation API
  slug: spare-bahrain-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-bahrain-pis-openapi-original.json
- filename: spare-ksa-authentication-openapi-original.json
  format: json
  label: Spare KSA Authentication API
  slug: spare-ksa-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-ksa-authentication-openapi-original.json
- filename: spare-ksa-ais-openapi-original.json
  format: json
  label: Spare KSA Account Information API
  slug: spare-ksa-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-ksa-ais-openapi-original.json
- filename: spare-ksa-pis-openapi-original.json
  format: json
  label: Spare KSA Payment Initiation API
  slug: spare-ksa-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-ksa-pis-openapi-original.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spare Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Spare secures its APIs with oauth2 and apiKey across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Spare
provider_slug: spare
scheme_count: 1
schemes:
- description: Please enter into field the word 'Bearer' followed by a space and JWT
  in: header
  name: Bearer
  parameter: Authorization
  scheme_semantics: OAuth2 JWT bearer token (obtained via client-credentials)
  sources:
  - openapi/spare-bahrain-ais-openapi-original.json
  - openapi/spare-bahrain-pis-openapi-original.json
  - openapi/spare-ksa-ais-openapi-original.json
  - openapi/spare-ksa-ais-v2-openapi-original.json
  - openapi/spare-ksa-pis-openapi-original.json
  type: apiKey
slug: spare-authentication
source_filename: spare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spare-bahrain-ais-openapi-original.json, openapi/spare-bahrain-pis-openapi-original.json,\n  openapi/spare-ksa-ais-openapi-original.json, openapi/spare-ksa-ais-v2-openapi-original.json,\n  openapi/spare-ksa-pis-openapi-original.json\ndocs: https://docs.tryspare.com/docs/auth-flow\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nmodel: >-\n  Spare uses OAuth2 client-credentials. A client presents its API credentials\n  (client id + client secret) to the Authentication API Token endpoint and\n  receives a signed JWT access token plus a refresh token. The access token is a\n  short-lived bearer token supplied on every protected request in the\n  Authorization header as `Bearer <JWT>`; when it expires the refresh token is\n  exchanged for a new access token via the Refresh endpoint. Token, payload and\n  webhook (x-signature) signatures are verified against\
  \ the tenant JWKS published\n  by the Authentication API. API keys are provisioned in the Dashboard as an\n  ECC secp256r1 (prime256v1) PKCS#8 key pair for request/message signing, with an\n  optional IP allow-list. Each tenant (Bahrain, KSA, UAE) is a separate host, so\n  tokens are tenant-scoped.\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_semantics: OAuth2 JWT bearer token (obtained via client-credentials)\n  description: Please enter into field the word 'Bearer' followed by a space and JWT\n  sources:\n  - openapi/spare-bahrain-ais-openapi-original.json\n  - openapi/spare-bahrain-pis-openapi-original.json\n  - openapi/spare-ksa-ais-openapi-original.json\n  - openapi/spare-ksa-ais-v2-openapi-original.json\n  - openapi/spare-ksa-pis-openapi-original.json\nendpoints:\n  token: /api/v1.0/authentication/Token\n  refresh: /api/v1.0/authentication/Refresh\n  jwks: /api/v1.0/authentication/Jwks\nmessage_signing:\n  algorithm: ECDSA (secp256r1\
  \ / prime256v1)\n  key_format: PKCS#8\n  provisioning: Dashboard - Developer Tools - Generate API Key (maker/checker approval)\nconsent_permissions: scopes/spare-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/authentication/spare-authentication.yml
summary_line: oauth2/apiKey · 1 scheme
tags:
- Open Banking
- Open Finance
- Account Information
- Payment Initiation
- AISP
- PISP
- Consent
- Bank Data
- Transactions
- Balances
- Payments
- Fintech
- MENA
- Saudi Arabia
- Bahrain
- UAE
---
