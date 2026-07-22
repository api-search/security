---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Runreveal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: RunReveal secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: RunReveal
provider_slug: runreveal
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://www-api.runreveal.com/oauth/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    - plain
    scope_count: 37
    tokenUrl: https://www-api.runreveal.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://www-api.runreveal.com/oauth/token
  name: OAuth2
  registration_endpoint: https://www-api.runreveal.com/oauth/client
  source: https://api.runreveal.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
  used_by: hosted remote MCP server (https://api.runreveal.com/mcp) and OAuth API clients
- description: Workspace-scoped API tokens created in the RunReveal console (scope tokens#create) authenticate the REST API, the CLI (`runreveal auth`), and the local MCP server (`runreveal mcp`). Tokens carry the workspace's RBAC permissions.
  in: header
  name: ApiToken
  scheme: bearer-token
  source: https://docs.runreveal.com/reference/using-the-cli
  type: apiKey
slug: runreveal-authentication
source_filename: runreveal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.runreveal.com/.well-known/oauth-authorization-server\ndocs: https://docs.runreveal.com/api-reference\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken]\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://api.runreveal.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www-api.runreveal.com/oauth/authorize\n    tokenUrl: https://www-api.runreveal.com/oauth/token\n    pkce_methods: [S256, plain]\n    scope_count: 37\n  - flow: refreshToken\n    tokenUrl: https://www-api.runreveal.com/oauth/token\n  registration_endpoint: https://www-api.runreveal.com/oauth/client\n  token_endpoint_auth_methods: [client_secret_post, none]\n  used_by: hosted remote MCP server (https://api.runreveal.com/mcp) and OAuth API clients\n- name: ApiToken\n  type: apiKey\n  in: header\n  scheme: bearer-token\n \
  \ source: https://docs.runreveal.com/reference/using-the-cli\n  description: >-\n    Workspace-scoped API tokens created in the RunReveal console (scope\n    tokens#create) authenticate the REST API, the CLI (`runreveal auth`), and\n    the local MCP server (`runreveal mcp`). Tokens carry the workspace's RBAC\n    permissions.\nnotes: >-\n  RunReveal also supports SAML/OIDC Single Sign-On for console login\n  (https://docs.runreveal.com/reference/single-sign-on) and SCIM user\n  provisioning; those govern human console access rather than API calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runreveal/refs/heads/main/authentication/runreveal-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Security
- SIEM
- Security Log Management
- Detection Engineering
- Threat Detection
- Incident Response
- Observability
- SQL
- MCP
- AI
---
