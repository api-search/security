---
api_key_in:
- header
api_specs:
- filename: unstoppable-finance-iron-openapi-original.yml
  format: yaml
  label: Iron API
  slug: iron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-iron-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Unstoppable Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unstoppable Finance (Iron) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unstoppable Finance (Iron)
provider_slug: unstoppable-finance
scheme_count: 1
schemes:
- description: 'API key created and managed in the Iron Partner Dashboard (Developer -> API Keys). Keys carry a role: Read Only or Read / Write. Missing, incorrect, or revoked keys return 401 Unauthorized with a plain-text authorization error. Separate keys per environment: sandbox keys at app.sandbox.iron.xyz/dashboard/keys, production keys at app.iron.xyz (production keys can only be created by an administrator).'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/unstoppable-finance-iron-openapi-original.yml
  type: apiKey
slug: unstoppable-finance-authentication
source_filename: unstoppable-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unstoppable-finance-iron-openapi-original.yml\ndocs: https://docs.iron.xyz/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key created and managed in the Iron Partner Dashboard (Developer -> API Keys). Keys carry a\n    role: Read Only or Read / Write. Missing, incorrect, or revoked keys return 401 Unauthorized with a plain-text\n    authorization error. Separate keys per environment: sandbox keys at app.sandbox.iron.xyz/dashboard/keys, production\n    keys at app.iron.xyz (production keys can only be created by an administrator).'\n  sources:\n  - openapi/unstoppable-finance-iron-openapi-original.yml\nnotes: All Iron API requests require the X-API-Key header. No OAuth2/OIDC surface. The Partner Dashboard itself\n  supports 2FA (docs.iron.xyz/2fa).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/authentication/unstoppable-finance-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Stablecoins
- Payments
- Onramp
- Offramp
- Cryptocurrency
- Banking
- Fintech
- Compliance
---
