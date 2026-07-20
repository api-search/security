---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Coro Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Coro secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Coro
provider_slug: coro
scheme_count: 1
schemes:
- audience: https://secure.coro.net/api
  credentials_source: Control Panel > Connectors > API Credentials in the Coro console (Client ID + Secret pair, distinct from console login). Up to 10 active credential sets; named, rotatable, and optionally given an expiration date.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_headers:
  - name: Authorization
    value: Bearer <access_token>
  - name: Workspace
    value: <WORKSPACE_ID>
  scopes: []
  scopes_note: No granular OAuth scopes are documented; a credential pair grants access scoped to its workspace and the admin role attached to it.
  token_endpoint: https://api.secure.coro.net/oauth/token
  token_endpoints_by_region:
    ca: https://api.secure-ca.coro.net/oauth/token
    eu: https://api.secure-eu.coro.net/oauth/token
    us: https://api.secure.coro.net/oauth/token
  token_ttl_seconds: 86400
  token_type: Bearer
  type: oauth2
slug: coro-authentication
source_filename: coro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.coro.net/developer-portal/authentication.md\ndocs: https://docs.coro.net/developer-portal/authentication/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  additional_required_headers: [Workspace]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://api.secure.coro.net/oauth/token\n  token_endpoints_by_region:\n    us: https://api.secure.coro.net/oauth/token\n    ca: https://api.secure-ca.coro.net/oauth/token\n    eu: https://api.secure-eu.coro.net/oauth/token\n  audience: https://secure.coro.net/api\n  grant_type: client_credentials\n  token_type: Bearer\n  token_ttl_seconds: 86400\n  credentials_source: >-\n    Control Panel > Connectors > API Credentials in the Coro console (Client ID +\n    Secret pair, distinct from console login). Up to 10 active credential sets;\n    named, rotatable, and optionally given an expiration date.\n\
  \  request_headers:\n  - name: Authorization\n    value: Bearer <access_token>\n  - name: Workspace\n    value: <WORKSPACE_ID>\n  scopes: []\n  scopes_note: >-\n    No granular OAuth scopes are documented; a credential pair grants access scoped\n    to its workspace and the admin role attached to it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coro/refs/heads/main/authentication/coro-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Security
- Endpoint Protection
- Email Security
- Cloud Security
- Data Protection
- MSP
- Webhooks
- MCP
---
