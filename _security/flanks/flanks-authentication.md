---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Flanks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flanks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flanks
provider_slug: flanks
scheme_count: 1
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request:
    content_type: application/json
    method: POST
    parameters:
    - client_id
    - client_secret
    - grant_type
  response:
    access_token: string
    expires_in: 3600
    scope: space-delimited list of scopes
    token_type: Bearer
  token_endpoint: https://api.flanks.io/v0/token
  type: oauth2
  usage: 'Every request carries header Authorization: Bearer <access_token>'
slug: flanks-authentication
source_filename: flanks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.flanks.io/pages/flanks-apis/authentication/\ndocs: https://docs.flanks.io/pages/flanks-apis/authentication/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  bearer: true\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://api.flanks.io/v0/token\n    grant_type: client_credentials\n    request:\n      method: POST\n      content_type: application/json\n      parameters:\n        - client_id\n        - client_secret\n        - grant_type\n    response:\n      access_token: string\n      token_type: Bearer\n      expires_in: 3600\n      scope: space-delimited list of scopes\n    usage: 'Every request carries header Authorization: Bearer <access_token>'\nnotes: >-\n  All Flanks API calls must be authenticated. Obtain a bearer access token from\n  the token endpoint using the OAuth2 client-credentials grant, then send it in\n  the\
  \ Authorization header. Access tokens expire after 3600 seconds. The hosted\n  Flanks MCP server uses a separate OAuth2 authorization server\n  (https://flanks-mcp.flanks.io) supporting authorization_code, refresh_token,\n  and client_credentials with PKCE (S256).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flanks/refs/heads/main/authentication/flanks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Wealth Management
- Financial Data
- Data Aggregation
- Fintech
- Investments
- Open Banking
- APIs
---
