---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Density Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Density secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Density
provider_slug: density
scheme_count: 2
schemes:
- description: Static, long-lived API token created by an account Owner in Atlas Developer Settings. Tokens are prefixed with "tok_" and passed in the Authorization header as "Bearer <token>". A request without a valid Authorization header returns 403.
  format: Bearer <token>
  header: Authorization
  name: bearerToken
  scheme: bearer
  sources:
  - docs
  token_prefix: tok_
  type: http
- description: Machine-to-machine OAuth 2.0 client-credentials flow (Auth0-backed). Create a Client ID / Client Secret in Atlas Developer Settings and exchange them at the token endpoint for a short-lived access token (JWT, prefixed "eyJ") passed as a Bearer token on subsequent requests.
  flows:
  - flow: clientCredentials
    grant_type: client_credentials
    tokenUrl: https://api.density.io/v3/oauth/token
    token_prefix: eyJ
  name: oauth2ClientCredentials
  sources:
  - docs
  type: oauth2
slug: density-authentication
source_filename: density-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.density.io/quick_start/\ndocs: https://developers.density.io/quick_start/\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  identity_provider: Auth0\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Static, long-lived API token created by an account Owner in Atlas Developer\n    Settings. Tokens are prefixed with \"tok_\" and passed in the Authorization\n    header as \"Bearer <token>\". A request without a valid Authorization header\n    returns 403.\n  header: Authorization\n  format: 'Bearer <token>'\n  token_prefix: tok_\n  sources: [docs]\n- name: oauth2ClientCredentials\n  type: oauth2\n  description: >-\n    Machine-to-machine OAuth 2.0 client-credentials flow (Auth0-backed). Create a\n    Client ID / Client Secret in Atlas Developer Settings and exchange them at the\n    token endpoint for a short-lived access token\
  \ (JWT, prefixed \"eyJ\") passed as a\n    Bearer token on subsequent requests.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.density.io/v3/oauth/token\n    grant_type: client_credentials\n    token_prefix: eyJ\n  sources: [docs]\nnotes:\n- An Owner role in the Density account is required to create API credentials (contact support@density.io).\n- Credentials are managed at https://atlas.density.io/ under Developer settings.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/density/refs/heads/main/authentication/density-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- Occupancy Sensors
- Workplace Analytics
- Real Time
- Occupancy
- Sensors
- IoT
- Space Utilization
- Proptech
---
