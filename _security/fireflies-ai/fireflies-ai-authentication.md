---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fireflies Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fireflies.ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fireflies.ai
provider_slug: fireflies-ai
scheme_count: 2
schemes:
- description: 'Standard bearer-token authentication. Include an Authorization header "Authorization: Bearer <API_KEY>" on every request to the GraphQL endpoint. API keys are generated in the Fireflies app under Settings > Developer Settings (Integrations > Fireflies API).'
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
- description: OAuth 2.0 authorization-code flow with PKCE (S256), used by the Fireflies MCP server and OAuth apps. Advertised via RFC 8414 metadata at /.well-known/oauth-authorization-server. Supports dynamic client registration and refresh tokens.
  flows:
  - authorizationUrl: https://api.fireflies.ai/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://api.fireflies.ai/register
    revocationUrl: https://api.fireflies.ai/revoke
    scopes:
      email: Access to the account email address.
      profile: Access to profile information.
    tokenUrl: https://api.fireflies.ai/token
  name: oauth2
  sources:
  - well-known/fireflies-ai-oauth-authorization-server.json
  type: oauth2
slug: fireflies-ai-authentication
source_filename: fireflies-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fireflies.ai/fundamentals/authorization\ndocs: https://docs.fireflies.ai/fundamentals/authorization\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  primary: bearer\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Standard bearer-token authentication. Include an Authorization header\n      \"Authorization: Bearer <API_KEY>\" on every request to the GraphQL endpoint.\n      API keys are generated in the Fireflies app under Settings > Developer\n      Settings (Integrations > Fireflies API).\n    location: header\n    header: Authorization\n    sources: [docs]\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization-code flow with PKCE (S256), used by the Fireflies\n      MCP server and OAuth apps. Advertised via RFC 8414 metadata at\n      /.well-known/oauth-authorization-server. Supports\
  \ dynamic client\n      registration and refresh tokens.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.fireflies.ai/authorize\n        tokenUrl: https://api.fireflies.ai/token\n        revocationUrl: https://api.fireflies.ai/revoke\n        registrationUrl: https://api.fireflies.ai/register\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\n        scopes:\n          profile: Access to profile information.\n          email: Access to the account email address.\n    sources: [well-known/fireflies-ai-oauth-authorization-server.json]\nnotes: >-\n  The GraphQL data API is documented as bearer-token only; OAuth 2.0 is the\n  authorization mechanism behind the hosted MCP server and third-party OAuth apps.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies-ai/refs/heads/main/authentication/fireflies-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Meetings
- Transcription
- Speech to Text
- Conversation Intelligence
- Artificial Intelligence
- GraphQL
- MCP
- Productivity
---
