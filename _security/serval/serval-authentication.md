---
api_key_in: []
api_specs:
- filename: serval-auth-openapi.yml
  format: yaml
  label: Serval Public API
  slug: serval-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serval/refs/heads/main/openapi/serval-auth-openapi.yml
auth_types:
- http-basic
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Serval Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Serval secures its APIs with http-basic, http-bearer, and oauth2 across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Serval
provider_slug: serval
scheme_count: 0
schemes: []
slug: serval-authentication
source_filename: serval-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.serval.com/api-reference/auth-api/create-token.md\ndocs: https://docs.serval.com/api-reference/auth-api/create-token\nsummary:\n  types: [http-basic, http-bearer, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\nmodels:\n  # 1. Public REST API v2 — machine-to-machine\n  - name: rest-api-token-exchange\n    audience: server-to-server integrations\n    scheme: http\n    description: >\n      Obtain an access token by POSTing grant_type=client_credentials to\n      https://public.api.serval.com/v2/auth/token with HTTP Basic auth\n      (username = Client ID, password = Client Secret, from app.serval.com/admin/settings).\n      The response returns access_token / token_type / expires_in. Use the token as\n      `Authorization: Bearer <access_token>` on all /v2/* requests.\n    token_endpoint: https://public.api.serval.com/v2/auth/token\n    schemes:\n      - name: basicAuth\n     \
  \   type: http\n        scheme: basic\n        use: token exchange (client_id:client_secret)\n        sources: [openapi/serval-auth-openapi.yml]\n      - name: bearerAuth\n        type: http\n        scheme: bearer\n        use: all subsequent API calls\n        sources: [openapi/serval-auth-openapi.yml]\n  # 2. OAuth 2.0 authorization server — the MCP / delegated-user surface\n  - name: oauth2-authorization-server\n    audience: interactive agents / MCP clients acting for a user\n    scheme: oauth2\n    description: >\n      RFC 8414 authorization server at public.api.serval.com powering the hosted MCP server.\n      Supports authorization_code with PKCE (S256), refresh_token, and jwt-bearer grants,\n      Dynamic Client Registration, and token revocation. Single scope: serval:user.\n    metadata: https://public.api.serval.com/.well-known/oauth-authorization-server\n    endpoints:\n      authorization: https://public.api.serval.com/oauth/authorize\n      token: https://public.api.serval.com/oauth/token\n\
  \      registration: https://public.api.serval.com/oauth/register\n      revocation: https://public.api.serval.com/oauth/revoke\n    grant_types: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    scopes: [serval:user]\nregions:\n  - {region: US, base: https://public.api.serval.com}\n  - {region: EU, base: https://public.eu1.serval.com}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serval/refs/heads/main/authentication/serval-authentication.yml
summary_line: http-basic/http-bearer/oauth2 · 0 schemes
tags:
- Company
- IT Service Management
- ITSM
- Help Desk
- Workflow Automation
- AI Agents
- Access Management
- Employee Support
- Ticketing
---
