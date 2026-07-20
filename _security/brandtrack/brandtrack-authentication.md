---
api_key_in:
- header
api_specs:
- filename: brandtrack-openapi-original.yml
  format: yaml
  label: Brandtrack API
  slug: brandtrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Brandtrack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Brandtrack secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Brandtrack
provider_slug: brandtrack
scheme_count: 3
schemes:
- description: Primary REST auth. Include an x-customer-api-key header on every authenticated request. Contact the Brandtrack team to obtain a key.
  in: header
  name: default
  parameter: x-customer-api-key
  sources:
  - openapi/brandtrack-openapi-original.yml
  type: apiKey
- description: Key used for the /partner/* endpoints (account registration, user token minting).
  in: header
  name: partner-key
  parameter: X-Partner-Key
  sources:
  - https://developers.brandtrack.ai/
  type: apiKey
- description: OAuth 2.0 authorization server discovered via RFC 8414 metadata at api.brandtrack.fm (.well-known/oauth-authorization-server). PKCE S256 required, single "mcp" scope — guards an MCP/agent access path. Not yet in the human docs.
  flows:
  - authorizationUrl: https://api.brandtrack.fm/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    revocationUrl: https://api.brandtrack.fm/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://api.brandtrack.fm/oauth/token
  name: OAuth2
  sources:
  - https://api.brandtrack.fm/.well-known/oauth-authorization-server
  type: oauth2
slug: brandtrack-authentication
source_filename: brandtrack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/brandtrack-openapi-original.yml + https://api.brandtrack.fm/.well-known/oauth-authorization-server\ndocs: https://developers.brandtrack.ai/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: default\n  type: apiKey\n  in: header\n  parameter: x-customer-api-key\n  description: >-\n    Primary REST auth. Include an x-customer-api-key header on every authenticated\n    request. Contact the Brandtrack team to obtain a key.\n  sources:\n  - openapi/brandtrack-openapi-original.yml\n- name: partner-key\n  type: apiKey\n  in: header\n  parameter: X-Partner-Key\n  description: Key used for the /partner/* endpoints (account registration, user token minting).\n  sources:\n  - https://developers.brandtrack.ai/\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.brandtrack.fm/oauth/authorize\n   \
  \ tokenUrl: https://api.brandtrack.fm/oauth/token\n    revocationUrl: https://api.brandtrack.fm/oauth/revoke\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    scopes: [mcp]\n  description: >-\n    OAuth 2.0 authorization server discovered via RFC 8414 metadata at\n    api.brandtrack.fm (.well-known/oauth-authorization-server). PKCE S256 required,\n    single \"mcp\" scope — guards an MCP/agent access path. Not yet in the human docs.\n  sources:\n  - https://api.brandtrack.fm/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/authentication/brandtrack-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Music
- Background Music
- Audio
- Streaming
- Retail
- Hospitality
- In-Store Experience
- Media
- Sound
---
