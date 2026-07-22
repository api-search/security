---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Qwilr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- tokenExchange
overview: Qwilr secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and tokenExchange flow(s).
provider_name: Qwilr
provider_slug: qwilr
scheme_count: 2
schemes:
- applies_to: https://api.qwilr.com/v1
  bearer_format: JWT
  description: REST API (https://api.qwilr.com/v1) authenticates with a bearer access token (JWT) in the Authorization header. Tokens are generated once in the Qwilr app at https://app.qwilr.com/#/settings/api and shown only a single time. API access requires an Enterprise Qwilr plan with API access enabled.
  name: bearerAuth
  scheme: bearer
  sources:
  - docs.qwilr.com/api-reference
  type: http
- applies_to: https://mcp.qwilr.com
  description: The hosted MCP server (https://mcp.qwilr.com) authenticates via OAuth 2.0 against the authorization server at https://api.qwilr.com, per RFC 8414 / RFC 9728 metadata. Supports authorization_code (PKCE S256), refresh_token, and RFC 8693 token-exchange grants; scope "mcp".
  flows:
  - authorizationUrl: https://api.qwilr.com/oauth/authorize
    flow: authorizationCode
    scopes:
      mcp: Access the Qwilr MCP server
    tokenUrl: https://api.qwilr.com/oauth/token
  name: mcpOAuth2
  sources:
  - api.qwilr.com/.well-known/oauth-authorization-server
  type: oauth2
slug: qwilr-authentication
source_filename: qwilr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qwilr.com/docs/getting-started/quick-start\ndocs: https://docs.qwilr.com/api-reference\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - tokenExchange\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    REST API (https://api.qwilr.com/v1) authenticates with a bearer access token\n    (JWT) in the Authorization header. Tokens are generated once in the Qwilr app\n    at https://app.qwilr.com/#/settings/api and shown only a single time. API\n    access requires an Enterprise Qwilr plan with API access enabled.\n  applies_to: https://api.qwilr.com/v1\n  sources:\n  - docs.qwilr.com/api-reference\n- name: mcpOAuth2\n  type: oauth2\n  description: >-\n    The hosted MCP server (https://mcp.qwilr.com) authenticates via OAuth 2.0\n    against the authorization server at https://api.qwilr.com, per RFC 8414 /\n\
  \    RFC 9728 metadata. Supports authorization_code (PKCE S256), refresh_token,\n    and RFC 8693 token-exchange grants; scope \"mcp\".\n  applies_to: https://mcp.qwilr.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.qwilr.com/oauth/authorize\n    tokenUrl: https://api.qwilr.com/oauth/token\n    scopes:\n      mcp: Access the Qwilr MCP server\n  sources:\n  - api.qwilr.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwilr/refs/heads/main/authentication/qwilr-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Proposals
- Documents
- Sales
- Quotes
- Contracts
- E-Signature
- Webhooks
- MCP
- SaaS
---
