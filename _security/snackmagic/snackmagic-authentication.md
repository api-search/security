---
api_key_in:
- header
api_specs:
- filename: snackmagic-stadium-openapi.yml
  format: yaml
  label: Stadium API (SnackMagic)
  slug: stadium-api-snackmagic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snackmagic/refs/heads/main/openapi/snackmagic-stadium-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Snackmagic Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- authorizationCodePKCE
- refreshToken
overview: SnackMagic secures its APIs with http, apiKey, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, authorizationCodePKCE, and refreshToken flow(s).
provider_name: SnackMagic
provider_slug: snackmagic
scheme_count: 2
schemes:
- applies_to: most endpoints (users, stores, orders, send_points)
  bearerFormat: JWT
  name: Token
  scheme: bearer
  sources:
  - openapi/snackmagic-stadium-openapi.yml
  type: http
- applies_to: webhook automation endpoints (/automations/orders, /automations/order_status)
  description: API key of the configured webhook automation.
  in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/snackmagic-stadium-openapi.yml
  type: apiKey
slug: snackmagic-authentication
source_filename: snackmagic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/snackmagic-stadium-openapi.yml\ndocs: https://api.bystadium.com/api/v2/docs\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - authorizationCodePKCE\n  - refreshToken\nnotes: >-\n  The Stadium API (SnackMagic is a Stadium brand) authorizes most endpoints with a\n  bearer JWT access token (the `Token` HTTP bearer scheme). Access tokens are obtained\n  through OAuth2 flows documented in the API description: Client Credentials (global\n  organizer accounts), Authorization Code (act on behalf of a Stadium user via\n  /oauth/authorize -> /oauth/token_by_code), Authorization Code with PKCE (native/SPA\n  clients), and refresh-token exchange. The webhook automation endpoints\n  (/automations/orders, /automations/order_status) instead authenticate with a static\n  `api_key` request header tied to a configured automation. The OpenAPI\
  \ only formally\n  declares the `Token` http-bearer scheme; the OAuth2 flows and the automation api_key\n  header are documented in prose and in the operation parameters, and are captured here.\nschemes:\n- name: Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: most endpoints (users, stores, orders, send_points)\n  sources:\n  - openapi/snackmagic-stadium-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  applies_to: webhook automation endpoints (/automations/orders, /automations/order_status)\n  description: API key of the configured webhook automation.\n  sources:\n  - openapi/snackmagic-stadium-openapi.yml\noauth2:\n  authorize_url: https://api.bystadium.com/api/v2/oauth/authorize\n  token_url: https://api.bystadium.com/api/v2/oauth/token\n  token_by_code_url: https://api.bystadium.com/api/v2/oauth/token_by_code\n  refresh_url: https://api.bystadium.com/api/v2/oauth/token_by_refresh_token\n  validate_url: https://api.bystadium.com/api/v2/oauth/validate\n\
  \  pkce: true\n  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snackmagic/refs/heads/main/authentication/snackmagic-authentication.yml
summary_line: http/apiKey/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Gifting
- Rewards
- Swag
- Snacks
- E-Commerce
- Fulfillment
---
