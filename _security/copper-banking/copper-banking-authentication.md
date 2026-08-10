---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Copper Banking Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Copper Banking secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Copper Banking
provider_slug: copper-banking
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://mcp.getcopper.com/authorize
    flow: authorizationCode
    scopes:
    - mcp
    - offline_access
    tokenUrl: https://mcp.getcopper.com/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.getcopper.com/
  name: CopperMCPOAuth2
  registration_endpoint: https://mcp.getcopper.com/register
  response_types:
  - code
  source: well-known/copper-banking-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: copper-banking-authentication
source_filename: copper-banking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://mcp.getcopper.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Copper publishes no developer documentation and no authentication guide. This profile\n  was derived entirely from the authorization server metadata document the MCP host\n  serves, plus the observed behaviour of its /authorize, /token and /register endpoints.\n  It could NOT be derived with derive-authentication.py because there is no OpenAPI in\n  this repo to read securitySchemes from.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  dynamic_client_registration: true\nschemes:\n- name: CopperMCPOAuth2\n  type: oauth2\n  source: well-known/copper-banking-oauth-authorization-server.json\n  issuer: https://mcp.getcopper.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.getcopper.com/authorize\n    tokenUrl: https://mcp.getcopper.com/token\n    scopes:\
  \ [mcp, offline_access]\n  registration_endpoint: https://mcp.getcopper.com/register\n  token_endpoint_auth_methods: [client_secret_post, none]\n  response_types: [code]\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\nobserved_behaviour:\n- endpoint: /authorize\n  method: GET\n  status: 400\n  body: '{\"error\":\"invalid_request\",\"error_description\":\"...\"}'\n  note: Validates query parameters and returns an RFC 6749 §4.1.2.1 error object.\n- endpoint: /token\n  method: GET\n  status: 405\n  body: '{\"error\":\"method_not_allowed\",...}'\n- endpoint: /token\n  method: POST\n  status: 400\n  body: '{\"error\":\"invalid_request\",...}'\n- endpoint: /register\n  method: POST\n  status: 400\n  body: '{\"error\":\"invalid_client_metadata\",...}'\n  note: RFC 7591 dynamic client registration is live and validates client metadata.\ngaps:\n- No /.well-known/oauth-protected-resource document (RFC 9728), so an MCP client cannot\n  discover the resource\
  \ server and its authorization servers from the resource itself.\n- No published documentation of the authentication flow, token lifetimes, or what the\n  `mcp` scope authorizes.\n- No API keys, no bearer-token guide, no public developer credentials of any kind —\n  Copper has no public developer program.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://mcp.getcopper.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-banking/refs/heads/main/authentication/copper-banking-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Financial Services
- Fintech
- Consumer Finance
- Financial Literacy
- Rewards
- Neobank
- Mobile Banking
- Teen Banking
- Model Context Protocol
---
