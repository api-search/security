---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Atlar Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Atlar secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Atlar
provider_slug: atlar
scheme_count: 3
schemes:
- access_token_ttl_seconds: 300
  credentials: Programmatic access user ACCESS_KEY as client_id and SECRET as client_secret. Supports client_secret_basic and client_secret_post.
  name: OAuth2ClientCredentials
  recommended: true
  scheme: clientCredentials
  tokenUrl: https://api.atlar.com/iam/v2/oauth2/token
  token_endpoint_v2beta: https://api.atlar.com/iam/v2beta/oauth2/token
  token_type: Bearer
  type: oauth2
- authorizationUrl: https://api.atlar.com/iam/v2/oauth2/authorize
  name: OAuth2AuthorizationCode
  pkce: S256
  scheme: authorizationCode
  tokenUrl: https://api.atlar.com/iam/v2/oauth2/token
  type: oauth2
  used_for: MCP CIMD clients (mcp.atlar.com), plus refresh_token grant
- credentials: ACCESS_KEY as username, SECRET as password
  name: HTTPBasic
  note: Supported but OAuth 2.0 access-token flow is recommended
  scheme: basic
  type: http
slug: atlar-authentication
source_filename: atlar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.atlar.com/docs/api\ndocs: https://docs.atlar.com/docs/accessing-the-api\nsummary:\n  types: [oauth2, http]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  well_known: https://api.atlar.com/.well-known/oauth-authorization-server\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    scheme: clientCredentials\n    tokenUrl: https://api.atlar.com/iam/v2/oauth2/token\n    token_endpoint_v2beta: https://api.atlar.com/iam/v2beta/oauth2/token\n    token_type: Bearer\n    access_token_ttl_seconds: 300\n    credentials: >-\n      Programmatic access user ACCESS_KEY as client_id and SECRET as\n      client_secret. Supports client_secret_basic and client_secret_post.\n    recommended: true\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    scheme: authorizationCode\n    authorizationUrl: https://api.atlar.com/iam/v2/oauth2/authorize\n    tokenUrl: https://api.atlar.com/iam/v2/oauth2/token\n\
  \    pkce: S256\n    used_for: MCP CIMD clients (mcp.atlar.com), plus refresh_token grant\n  - name: HTTPBasic\n    type: http\n    scheme: basic\n    credentials: ACCESS_KEY as username, SECRET as password\n    note: Supported but OAuth 2.0 access-token flow is recommended\nnotes: >-\n  Bearer access tokens are passed as `Authorization: Bearer <token>`. Tokens are\n  short-lived (expires_in = 300s). Programmatic access users are created in the\n  Atlar Dashboard. Organizations gate agent/third-party OAuth via a Read-only or\n  Read-and-write access policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/authentication/atlar-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Fintech
- Treasury
- Payments
- Banking
- Cash Management
- Financial Operations
- ERP Integration
---
