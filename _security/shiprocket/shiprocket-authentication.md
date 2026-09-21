---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shiprocket-api-openapi.yml
  format: yaml
  label: Shiprocket API
  slug: shiprocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiprocket/refs/heads/main/openapi/shiprocket-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Shiprocket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shiprocket secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shiprocket
provider_slug: shiprocket
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT obtained from POST /v1/external/auth/login with an API user email + password. Sent as Authorization: Bearer <token> on every other call.'
  logout_endpoint: https://apiv2.shiprocket.in/v1/external/auth/logout
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shiprocket-api-openapi.yml
  - https://apidocs.shiprocket.in/
  token_endpoint: https://apiv2.shiprocket.in/v1/external/auth/login
  token_ttl: 10 days
  type: http
slug: shiprocket-authentication
source_filename: shiprocket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: openapi/shiprocket-api-openapi.yml + https://apidocs.shiprocket.in/ (Getting Started, Authentication API)\ndocs: https://apidocs.shiprocket.in/\nsummary:\n  types:\n  - http\n  style: login-for-JWT bearer\n  oauth2: false\n  openid: false\n  api_keys: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT obtained from POST /v1/external/auth/login with an API user email + password. Sent as Authorization:\n    Bearer <token> on every other call.'\n  token_endpoint: https://apiv2.shiprocket.in/v1/external/auth/login\n  logout_endpoint: https://apiv2.shiprocket.in/v1/external/auth/logout\n  token_ttl: 10 days\n  sources:\n  - openapi/shiprocket-api-openapi.yml\n  - https://apidocs.shiprocket.in/\ncredential_provisioning:\n  where: Shiprocket panel > Settings > API > Add New API User\n  steps:\n  - Create an API user with a unique email (must differ from the main login).\n\
  \  - 'Select the API modules the user may access (\"Modules to Access\") and whether buyer details are exposed (\"Buyer''s\n    Details Access\": Allowed / Not Allowed).'\n  - Copy the generated API password immediately — it is shown once.\n  - Exchange email + password at POST /v1/external/auth/login for the JWT.\n  scoping: module-level access per API user; no OAuth scopes\n  sandbox: none — the docs warn that any request with valid credentials affects live account data\nnotes: No OAuth 2.0 or OpenID Connect on the logistics API. (The separate WordPress MCP endpoint on www.shiprocket.in\n  uses OAuth 2.1 with PKCE and scope \"mcp\" — see well-known/ and mcp/.)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiprocket/refs/heads/main/authentication/shiprocket-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Shipping
- Logistics
- E-Commerce
- Fulfillment
- Last Mile Delivery
- Order Management
- Courier Aggregation
- India
---
