---
api_key_in: []
api_specs:
- filename: treasuryspring-openapi-original.json
  format: json
  label: TreasurySpring Public API
  slug: treasuryspring-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Treasuryspring Authentication
name_suffix: Authentication
oauth_flows: []
overview: TreasurySpring secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TreasurySpring
provider_slug: treasuryspring
scheme_count: 2
schemes:
- description: 'Base64-encoded `client_id:client_secret` (sent as `Authorization: Basic <base64>`). Used by the OAuth token-exchange endpoint.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/treasuryspring-openapi-original.json
  type: http
- description: 'API Key or OAuth access token (sent as `Authorization: Bearer <token>`).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/treasuryspring-openapi-original.json
  type: http
slug: treasuryspring-authentication
source_filename: treasuryspring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/treasuryspring-openapi-original.json\ndocs: https://docs.treasuryspring.com/\nnotes: >-\n  REST API uses OAuth 2.0 client-credentials: exchange base64 client_id:client_secret\n  (HTTP Basic) at POST /oauth/token for a Bearer access token (access_token,\n  expires_in, refresh_token). All other endpoints take Authorization: Bearer <token>\n  (an API Key or OAuth access token). The published MCP server uses the OAuth 2.0\n  authorization-code flow with PKCE backed by Auth0, and advertises Dynamic Client\n  Registration (RFC 7591) so clients need no pre-configured client_id.\noauth2:\n  grant_types: [client_credentials, authorization_code]\n  token_endpoint: https://api.treasuryspring.com/api/v1/oauth/token\n  pkce: true\n  dynamic_client_registration: true\n  identity_provider: Auth0\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Base64-encoded `client_id:client_secret`\
  \ (sent as `Authorization: Basic <base64>`).\n    Used by the OAuth token-exchange endpoint.'\n  sources:\n  - openapi/treasuryspring-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API Key or OAuth access token (sent as `Authorization: Bearer <token>`).'\n  sources:\n  - openapi/treasuryspring-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/authentication/treasuryspring-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Fintech
- Cash Management
- Treasury
- Investments
- Financial Services
- Fixed Term Funds
- Payments
- MCP
---
