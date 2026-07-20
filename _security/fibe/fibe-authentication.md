---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fibe Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fibe secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fibe
provider_slug: fibe
scheme_count: 1
schemes:
- applies_to: Fibe MCP server (https://www.fibe.in/api/mcp)
  bearer:
    scheme: Bearer
    where: header
  flows:
  - authorizationUrl: https://www.fibe.in/api/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://www.fibe.in/api/mcp/oauth/register
    scopes:
      loan.apply: Submit or initiate a loan application
      loan.read: Read loan / eligibility information
    tokenUrl: https://www.fibe.in/api/mcp/oauth/token
  name: OAuth2
  type: oauth2
slug: fibe-authentication
source_filename: fibe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.fibe.in/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth: none    # public clients\nschemes:\n- name: OAuth2\n  type: oauth2\n  applies_to: Fibe MCP server (https://www.fibe.in/api/mcp)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fibe.in/api/mcp/oauth/authorize\n    tokenUrl: https://www.fibe.in/api/mcp/oauth/token\n    registrationUrl: https://www.fibe.in/api/mcp/oauth/register\n    code_challenge_methods: [S256]\n    scopes:\n      loan.read: Read loan / eligibility information\n      loan.apply: Submit or initiate a loan application\n  bearer:\n    where: header\n    scheme: Bearer\nnotes: >-\n  Fibe's only public machine-facing surface is its MCP server, protected by OAuth 2.0\n  authorization-code flow with PKCE (S256) and RFC 7591 dynamic client registration.\n\
  \  No REST/OpenAPI or API-key surface is published. The consumer web/app portal\n  (portal.fibe.in) uses a separate session login not documented for programmatic use.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fibe/refs/heads/main/authentication/fibe-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Lending
- Personal Loans
- Consumer Finance
- India
- Credit
- MCP
- Agent
---
