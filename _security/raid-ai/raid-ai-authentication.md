---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Raid Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- refreshToken
overview: Raid AI secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, and refreshToken flow(s).
provider_name: Raid AI
provider_slug: raid-ai
scheme_count: 3
schemes:
- description: Every request to the Raid AI detection API is authenticated with a secret API token, created in the dashboard (API Keys -> Create Key). A key is granted one or more detection scopes and an optional expiry, and the token is shown only once. A missing/invalid/revoked/expired key returns 401 Unauthorized; calling an endpoint the key is not scoped for returns 403 Forbidden. Tokens are server-side secrets — never embed in client code.
  format: 'Authorization: Bearer <your-token>'
  header: Authorization
  in: header
  name: apiToken
  scheme: bearer
  source: docs.raidxai.com/docs/authentication
  type: http
- description: Platform / dashboard identity is an OpenIddict OAuth 2.0 + OpenID Connect server (separate from the API-key surface used to call detection endpoints). Discovery advertises authorization, token, introspection, userinfo and logout endpoints and RS256-signed ID tokens.
  name: OpenIDConnect
  openIdConnectUrl: https://api.raidxai.com/.well-known/openid-configuration
  source: api.raidxai.com/.well-known/openid-configuration
  type: openIdConnect
- flows:
  - authorizationUrl: https://api.raidxai.com/connect/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://api.raidxai.com/connect/token
  - flow: clientCredentials
    tokenUrl: https://api.raidxai.com/connect/token
  - flow: password
    tokenUrl: https://api.raidxai.com/connect/token
  name: OAuth2
  source: api.raidxai.com/.well-known/openid-configuration
  type: oauth2
slug: raid-ai-authentication
source_filename: raid-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.raidxai.com/docs/authentication\ndocs: https://docs.raidxai.com/docs/authentication\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  api_key_scheme: bearer\n  oauth2_flows: [authorizationCode, clientCredentials, password, refreshToken]\nschemes:\n  - name: apiToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Authorization: Bearer <your-token>\"\n    description: >-\n      Every request to the Raid AI detection API is authenticated with a secret\n      API token, created in the dashboard (API Keys -> Create Key). A key is\n      granted one or more detection scopes and an optional expiry, and the token\n      is shown only once. A missing/invalid/revoked/expired key returns 401\n      Unauthorized; calling an endpoint the key is not scoped for returns 403\n      Forbidden. Tokens are server-side secrets — never embed in client code.\n\
  \    source: docs.raidxai.com/docs/authentication\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://api.raidxai.com/.well-known/openid-configuration\n    description: >-\n      Platform / dashboard identity is an OpenIddict OAuth 2.0 + OpenID Connect\n      server (separate from the API-key surface used to call detection\n      endpoints). Discovery advertises authorization, token, introspection,\n      userinfo and logout endpoints and RS256-signed ID tokens.\n    source: api.raidxai.com/.well-known/openid-configuration\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.raidxai.com/connect/authorize\n        tokenUrl: https://api.raidxai.com/connect/token\n        pkce: [S256, plain]\n      - flow: clientCredentials\n        tokenUrl: https://api.raidxai.com/connect/token\n      - flow: password\n        tokenUrl: https://api.raidxai.com/connect/token\n    source: api.raidxai.com/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raid-ai/refs/heads/main/authentication/raid-ai-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Deepfake Detection
- AI Content Detection
- Media Forensics
- Voice / Audio Detection
- Image Forensics
- Document Forensics
- Fact-Checking
- Trust & Safety
- Security
---
