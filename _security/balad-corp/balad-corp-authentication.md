---
api_key_in: []
api_specs:
- filename: balad-corp-gateway-openapi.yml
  format: yaml
  label: Balad Gateway API
  slug: balad-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-gateway-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Balad Corp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BALAD CORP secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BALAD CORP
provider_slug: balad-corp
scheme_count: 1
schemes:
- expires_in_seconds: 3600
  flow: clientCredentials
  grant_type: client_credentials
  header: 'Authorization: Bearer <ACCESS_TOKEN>'
  name: OAuth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  request_fields:
  - grant_type
  - client_id
  - client_secret
  response_fields:
  - access_token
  - token_type
  - expires_in
  - scope
  scope_note: Tokens are scoped to specific product APIs (remittances, collections, bills, vouchers). Balad does not publish an enumerated scope reference; scope is returned on the token response.
  scoped: true
  sources:
  - openapi/balad-corp-gateway-openapi.yml
  token_endpoint: /identity/v1/token
  token_type: Bearer
  type: oauth2
slug: balad-corp-authentication
source_filename: balad-corp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.balad.tech/authorization-1459814m0.md\ndocs: https://developers.balad.tech/authorization-1459814m0.md\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  server_to_server: true\n  transport: Bearer access token in Authorization header\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: /identity/v1/token\n    grant_type: client_credentials\n    request_content_type: application/x-www-form-urlencoded\n    request_fields: [grant_type, client_id, client_secret]\n    response_fields: [access_token, token_type, expires_in, scope]\n    token_type: Bearer\n    expires_in_seconds: 3600\n    header: 'Authorization: Bearer <ACCESS_TOKEN>'\n    scoped: true\n    scope_note: >-\n      Tokens are scoped to specific product APIs (remittances, collections, bills, vouchers).\n      Balad does not publish an enumerated scope reference; scope is\
  \ returned on the token response.\n    sources: [openapi/balad-corp-gateway-openapi.yml]\nnotes:\n  credentials: >-\n    Client ID and Client Secret are issued during partner onboarding and managed from the\n    Balad Dashboard (Developer -> Client Secrets). A maximum of 5 active secrets is allowed.\n  ip_whitelisting: >-\n    Production API access is IP-restricted; partners must supply static IP(s) to be whitelisted\n    before authenticating against production APIs (see Go Live).\n  revocation: Access tokens/secrets can be revoked instantly from the Balad Dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/authentication/balad-corp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Remittances
- Cross-Border Payments
- Fintech
- Egypt
- Payouts
- Money Transfer
- Banking
- API
---
