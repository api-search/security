---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Thoropass Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Thoropass secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Thoropass
provider_slug: thoropass
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://app.thoropass.com/partner-api
    flow: authorizationCode
    refreshUrl: https://api.thoropass.com/oauth/token/
    tokenUrl: https://api.thoropass.com/oauth/token/
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://api.thoropass.com
  name: OAuth2
  registration_endpoint: https://api.thoropass.com/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://api.thoropass.com/oauth/revoke-token/
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: thoropass-authentication
source_filename: thoropass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.thoropass.com/.well-known/oauth-authorization-server\ndocs: https://docs.thoropass.com/mcp\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  issuer: https://api.thoropass.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.thoropass.com/partner-api\n    tokenUrl: https://api.thoropass.com/oauth/token/\n    refreshUrl: https://api.thoropass.com/oauth/token/\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  revocation_endpoint: https://api.thoropass.com/oauth/revoke-token/\n  registration_endpoint: https://api.thoropass.com/oauth/register   # RFC 7591 dynamic client registration\n\
  notes: >-\n  Thoropass Partner API uses OAuth 2.0 Authorization Code with PKCE (S256) and\n  refresh tokens. Public clients are supported (token_endpoint_auth_method \"none\")\n  alongside confidential clients (client_secret_basic/post). Dynamic client\n  registration (RFC 7591) is offered. Scope reference: scopes/thoropass-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thoropass/refs/heads/main/authentication/thoropass-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Compliance
- Compliance Automation
- Audit
- Security
- Cybersecurity
- GRC
- SOC 2
- MCP
---
