---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Unwrap Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Unwrap secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Unwrap
provider_slug: unwrap
scheme_count: 2
schemes:
- applies_to: GraphQL data API
  description: 'Personal API key generated from the Unwrap user profile, sent as "Authorization: Bearer <UNWRAP_ACCESS_KEY>". Each token is scoped to a specific View (team_id); tokens expire if an org admin removes the member. Endpoint: https://data.api.production.unwrap.ai/'
  name: bearerAuth
  scheme: bearer
  source: https://docs.unwrap.ai/articles/6140971517-getting-started
  type: http
- applies_to: MCP / NLP API (nlp.api.production.unwrap.ai)
  description: OAuth 2.0 authorization for the Unwrap MCP server; supports dynamic client registration and static enterprise credentials.
  flows:
  - authorizationUrl: https://nlp.api.production.unwrap.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token
  - flow: clientCredentials
    tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token
  - flow: refreshToken
    tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token
  name: oauth2
  source: well-known/unwrap-openid-configuration.json
  type: oauth2
slug: unwrap-authentication
source_filename: unwrap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.unwrap.ai/articles/6140971517-getting-started\ndocs: https://docs.unwrap.ai/collections/6774268412-api\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  note: >-\n    The GraphQL data API authenticates with a personal API key sent as an HTTP\n    Bearer token. The MCP / NLP API authenticates via OAuth 2.0 (PKCE), with\n    discovery published at nlp.api.production.unwrap.ai/.well-known/.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Personal API key generated from the Unwrap user profile, sent as\n      \"Authorization: Bearer <UNWRAP_ACCESS_KEY>\". Each token is scoped to a\n      specific View (team_id); tokens expire if an org admin removes the\n      member. Endpoint: https://data.api.production.unwrap.ai/\n    applies_to: GraphQL data API\n    source: https://docs.unwrap.ai/articles/6140971517-getting-started\n\
  \  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization for the Unwrap MCP server; supports dynamic\n      client registration and static enterprise credentials.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://nlp.api.production.unwrap.ai/oauth/authorize\n        tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token\n      - flow: refreshToken\n        tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token\n    applies_to: MCP / NLP API (nlp.api.production.unwrap.ai)\n    source: well-known/unwrap-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unwrap/refs/heads/main/authentication/unwrap-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai Apps
- Customer Feedback
- Customer Intelligence
- Product Analytics
- Voice of Customer
- NLP
- GraphQL
- MCP
---
