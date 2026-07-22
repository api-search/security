---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nova Lima Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nova Lima secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nova Lima
provider_slug: nova-lima
scheme_count: 3
schemes:
- description: Account-level key that identifies the whole account. Cannot be changed through the GUI.
  in: header
  name: AppKey
  parameter_name: App-Key
  sources:
  - https://runrun.it/api/documentation
  type: apiKey
- description: Per-user token allowing an agent to act on behalf of that user.
  in: header
  name: UserToken
  parameter_name: User-Token
  sources:
  - https://runrun.it/api/documentation
  type: apiKey
- flows:
  - authorizationUrl: https://runrun.it/api/v1.0/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://runrun.it/mcp/oauth/register
    revocationUrl: https://runrun.it/api/v1.0/oauth/revoke
    scopes:
      all: Full access (the only scope advertised by the authorization server)
    tokenUrl: https://runrun.it/api/v1.0/oauth/token
  name: OAuth2
  sources:
  - https://runrun.it/.well-known/oauth-authorization-server
  type: oauth2
slug: nova-lima-authentication
source_filename: nova-lima-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://runrun.it/api/documentation\ndocs: https://runrun.it/api/documentation\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The primary REST API authenticates with two static header credentials:\n    App-Key (identifies the whole account, not changeable through the GUI) and\n    User-Token (unique per user; lets an agent act on behalf of that user).\n    Both headers must be sent on every request; an incorrect App-Key or\n    User-Token returns 401 Unauthorized. API access is a premium feature limited\n    to certain paid plans. Separately, runrun.it operates an OAuth 2.0/2.1\n    authorization server (authorization code + PKCE S256) used by the hosted MCP\n    server and OAuth clients.\nschemes:\n  - name: AppKey\n    type: apiKey\n    in: header\n    parameter_name: App-Key\n    description: Account-level key that identifies the whole account. Cannot be\
  \ changed through the GUI.\n    sources: [https://runrun.it/api/documentation]\n  - name: UserToken\n    type: apiKey\n    in: header\n    parameter_name: User-Token\n    description: Per-user token allowing an agent to act on behalf of that user.\n    sources: [https://runrun.it/api/documentation]\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://runrun.it/api/v1.0/oauth/authorize\n        tokenUrl: https://runrun.it/api/v1.0/oauth/token\n        revocationUrl: https://runrun.it/api/v1.0/oauth/revoke\n        registrationUrl: https://runrun.it/mcp/oauth/register\n        pkce: S256\n        scopes:\n          all: Full access (the only scope advertised by the authorization server)\n    sources: [https://runrun.it/.well-known/oauth-authorization-server]\nwhere_to_get_keys: >-\n  In the Runrun.it app: open \"Integration and Apps\", find \"API and Webhooks\",\n  click Open. The App-Key is displayed next to the User-Token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-lima/refs/heads/main/authentication/nova-lima-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Project Management
- Task Management
- Work Management
- Productivity
- Time Tracking
- Team Collaboration
- SaaS
- Brazil
---
