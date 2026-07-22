---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Versa Networks Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Versa Networks secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Versa Networks
provider_slug: versa-networks
scheme_count: 3
schemes:
- flow: password
  name: OAuth2Password
  notes: 'Recommended by Versa for REST API access. A client (client_id/client_secret) is registered, then exchanged with user credentials at /auth/token for a bearer access token used as `Authorization: Bearer <token>`. Confirmed in the first-party MCP server (vnmcpserver) auth flow.'
  parameters:
  - client_id
  - client_secret
  - username
  - password
  - grant_type=password
  port: 9183
  recommended: true
  returns: access_token (JWT bearer) + refresh_token
  scheme: oauth2
  token_url: /auth/token
  type: oauth2
- name: BasicAuth
  notes: HTTP Basic authentication (username:password) on port 9182. Per Versa docs, releases 23.1.1 and later support only basicAuth for some endpoints; OAuth is recommended where available.
  port: 9182
  scheme: basic
  type: http
- bearer_format: JWT
  name: BearerAuth
  notes: Bearer token obtained from the OAuth2 password flow; sent on all subsequent requests.
  scheme: bearer
  type: http
slug: versa-networks-authentication
source_filename: versa-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.versa-networks.com/Management_and_Orchestration/Versa_Director/Director_REST_APIs/Versa_Director_REST_API_Overview\ndocs: https://docs.versa-networks.com/Management_and_Orchestration/Versa_Director/Director_REST_APIs/Versa_Director_REST_API_Overview\nsummary:\n  types: [oauth2, http]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [password]\n  api_key_in: []\nschemes:\n  - name: OAuth2Password\n    type: oauth2\n    scheme: oauth2\n    flow: password\n    token_url: /auth/token\n    port: 9183\n    parameters: [client_id, client_secret, username, password, grant_type=password]\n    returns: access_token (JWT bearer) + refresh_token\n    recommended: true\n    notes: >-\n      Recommended by Versa for REST API access. A client (client_id/client_secret)\n      is registered, then exchanged with user credentials at /auth/token for a\n      bearer access token used as `Authorization: Bearer <token>`. Confirmed in\
  \ the\n      first-party MCP server (vnmcpserver) auth flow.\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    port: 9182\n    notes: >-\n      HTTP Basic authentication (username:password) on port 9182. Per Versa docs,\n      releases 23.1.1 and later support only basicAuth for some endpoints; OAuth is\n      recommended where available.\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    notes: Bearer token obtained from the OAuth2 password flow; sent on all subsequent requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versa-networks/refs/heads/main/authentication/versa-networks-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Networking
- Security
- SASE
- SD-WAN
- SSE
- Zero Trust
- ZTNA
- Cybersecurity
- Cloud Networking
- Infrastructure
- MCP
---
