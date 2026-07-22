---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Allstacks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Allstacks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Allstacks
provider_slug: allstacks
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.allstacks.com/oauth/authorize/
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://app.allstacks.com/oauth/register/
    scopes:
    - connector
    tokenUrl: https://app.allstacks.com/oauth/token/
    token_endpoint_auth_methods:
    - none
  issuer: https://app.allstacks.com
  name: OAuth2
  source: well-known/allstacks-oauth-authorization-server.json
  type: oauth2
slug: allstacks-authentication
source_filename: allstacks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://app.allstacks.com/.well-known/oauth-authorization-server\ndocs: https://app.allstacks.com/.well-known/oauth-protected-resource\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\n  bearer_methods: [header]\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: well-known/allstacks-oauth-authorization-server.json\n  issuer: https://app.allstacks.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.allstacks.com/oauth/authorize/\n    tokenUrl: https://app.allstacks.com/oauth/token/\n    registrationUrl: https://app.allstacks.com/oauth/register/\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    grant_types: [authorization_code, refresh_token]\n    scopes:\n    - connector\nnotes: >-\n  Derived from Allstacks' live RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata on app.allstacks.com.\
  \ Access is OAuth 2.0\n  authorization-code with mandatory PKCE (S256) and RFC 7591 dynamic client\n  registration; protected resources accept bearer tokens via the Authorization\n  header. A single \"connector\" scope is advertised. No public OpenAPI is published,\n  so this profile is grounded in the well-known discovery documents rather than a\n  spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allstacks/refs/heads/main/authentication/allstacks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Software Engineering Intelligence
- Value Stream Management
- Developer Productivity
- DevOps
- Analytics
- AI Agents
---
