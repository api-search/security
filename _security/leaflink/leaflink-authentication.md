---
api_key_in:
- header
api_specs:
- filename: leaflink-api-openapi-original.yml
  format: yaml
  label: LeafLink API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/openapi/leaflink-api-openapi-original.yml
- filename: leaflink-marketplace-v2-openapi-original.yml
  format: yaml
  label: LeafLink Marketplace V2 API
  slug: marketplace-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/openapi/leaflink-marketplace-v2-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Leaflink Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeafLink secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeafLink
provider_slug: leaflink
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Authentication is done via access tokens (JWTs). See the [API authentication doc](/api/getting-started/#authentication) for more information.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/leaflink-api-openapi-original.yml
  type: http
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/leaflink-api-openapi-original.yml
  - openapi/leaflink-marketplace-v2-openapi-original.yml
  type: apiKey
slug: leaflink-authentication
source_filename: leaflink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://developer.leaflink.com/api/getting-started/ (docs) + openapi/leaflink-api-openapi-original.yml,\n  openapi/leaflink-marketplace-v2-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Authentication is done via access tokens (JWTs). See the [API authentication doc](/api/getting-started/#authentication)\n    for more information.\n  sources:\n  - openapi/leaflink-api-openapi-original.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/leaflink-api-openapi-original.yml\n  - openapi/leaflink-marketplace-v2-openapi-original.yml\ndocs:\n- https://developer.leaflink.com/api/getting-started/\n- https://developer.leaflink.com/legacy/v2/api/authorization/\n\
  - https://help.leaflink.com/s/article/How-to-Create-API-Keys-and-Webhooks-in-LeafLink\ndocumented:\n  current_api:\n    api: LeafLink API\n    scheme: http bearer\n    format: JWT\n    header: 'Authorization: Bearer <YOUR_JWT>'\n    unauthenticated_response: 401\n    docs: https://developer.leaflink.com/api/getting-started/\n  legacy_v2:\n    api: LeafLink Marketplace V2 API\n    scheme: apiKey in header\n    header: 'Authorization: App <api_key>'\n    alternate_prefix: Token\n    note: Exactly one space separates the prefix from the key.\n    docs: https://developer.leaflink.com/legacy/v2/api/authorization/\ncredential_types:\n- name: User Token\n  scope: every company the token holder has permissions for in LeafLink\n- name: App Token\n  scope: only the single company where the token was created\ncredential_issuance:\n  self_service: true\n  how: A user generates an API key in the LeafLink dashboard under Settings > Developer Options; an admin must first\n    enable \"Developer access\"\
  \ and grant the permission.\n  docs: https://help.leaflink.com/s/article/How-to-Create-API-Keys-and-Webhooks-in-LeafLink\n  support: https://developer.leaflink.com/support/\n  ownership: The user who generates the key becomes its \"owner\" for rate-limiting purposes.\noauth:\n  supported: false\n  note: LeafLink uses key/JWT-based authentication only — no OAuth 2.0 or OIDC. No scopes/ artifact is emitted.\nscopes:\n  published: false\n  note: No scope or permission surface is exposed through the API; access is bounded by the token type and the company/role\n    the key was issued under.\ntransport:\n  https_only: true\n  cors: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/authentication/leaflink-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cannabis
- Wholesale
- B2B Marketplace
- Supply Chain
- Payments
- Logistics
- Inventory
- Compliance
- Traceability
- eCommerce
- Distribution
- Retail
---
