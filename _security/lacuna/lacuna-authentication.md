---
api_key_in:
- header
api_specs:
- filename: lacuna-lacuna-music-api-api-openapi.yml
  format: yaml
  label: Lacuna Lacuna Music API API
  slug: lacuna-lacuna-music-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-lacuna-music-api-api-openapi.yml
- filename: lacuna-music-api-openapi.yml
  format: yaml
  label: Lacuna Music API
  slug: lacuna-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-music-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lacuna Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lacuna secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lacuna
provider_slug: lacuna
scheme_count: 2
schemes:
- description: 'Lacuna developer API key issued from the dashboard at /profile/api and sent as `Authorization: Bearer lyr_live_...`. Shown once at creation. Keys carry scopes and an optional expiry set at creation time; revocation at the same URL takes effect immediately. Requires an active Pro plan or above — the tier check runs on every request, so a downgrade invalidates live keys without revoking them (403 permission_error / tier_insufficient).'
  key_prefix: lyr_live_
  name: bearerAuth
  registration_url: https://www.lacuna.fm/profile/api
  requires_human_interaction: true
  scheme: bearer
  sources:
  - openapi/lacuna-music-openapi-original.json
  - well-known/lacuna-auth.md
  - a2a/lacuna-agent-card.json
  - mcp/lacuna-mcp-server-card.json
  type: http
- description: OAuth 2.0 authorization code flow with PKCE (S256 required) for first-party clients registered manually with Lacuna. Public clients — token_endpoint_auth_method is `none`. Access tokens live 15 minutes; refresh tokens are issued to the iOS client only.
  dynamic_client_registration: false
  flows:
  - authorizationUrl: https://www.lacuna.fm/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    revocationUrl: https://www.lacuna.fm/oauth/revoke
    scopes: 5
    tokenUrl: https://www.lacuna.fm/oauth/token
  name: oauth2
  sources:
  - well-known/lacuna-oauth-authorization-server.json
  - well-known/lacuna-auth.md
  - a2a/lacuna-agent-card.json
  type: oauth2
slug: lacuna-authentication
source_filename: lacuna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/lacuna-music-openapi-original.json\ndocs: https://www.lacuna.fm/auth.md\ndiscovery:\n  authorization_server_metadata: https://www.lacuna.fm/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://www.lacuna.fm/.well-known/oauth-protected-resource\n  jwks_uri: https://www.lacuna.fm/.well-known/jwks.json\n  agent_auth_guide: https://www.lacuna.fm/auth.md\nsummary:\n  types:\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n  anonymous_tier: false\n  notes: >-\n    Two credential paths, both requiring a human account holder at some point: a developer API key\n    (recommended for autonomous agents, the only browser-free path) or OAuth 2.0 authorization code\n    with PKCE for manually-registered first-party clients. Dynamic client registration (RFC 7591) is\n    explicitly NOT supported. The same Authorization: Bearer header is used across REST, MCP\
  \ and A2A.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Lacuna developer API key issued from the dashboard at /profile/api and sent as\n      `Authorization: Bearer lyr_live_...`. Shown once at creation. Keys carry scopes and an optional\n      expiry set at creation time; revocation at the same URL takes effect immediately. Requires an\n      active Pro plan or above — the tier check runs on every request, so a downgrade invalidates\n      live keys without revoking them (403 permission_error / tier_insufficient).\n    key_prefix: lyr_live_\n    registration_url: https://www.lacuna.fm/profile/api\n    requires_human_interaction: true\n    sources:\n      - openapi/lacuna-music-openapi-original.json\n      - well-known/lacuna-auth.md\n      - a2a/lacuna-agent-card.json\n      - mcp/lacuna-mcp-server-card.json\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization code flow with PKCE (S256 required) for\
  \ first-party clients registered\n      manually with Lacuna. Public clients — token_endpoint_auth_method is `none`. Access tokens live\n      15 minutes; refresh tokens are issued to the iOS client only.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.lacuna.fm/oauth/authorize\n        tokenUrl: https://www.lacuna.fm/oauth/token\n        revocationUrl: https://www.lacuna.fm/oauth/revoke\n        code_challenge_methods_supported:\n          - S256\n        scopes: 5\n    dynamic_client_registration: false\n    sources:\n      - well-known/lacuna-oauth-authorization-server.json\n      - well-known/lacuna-auth.md\n      - a2a/lacuna-agent-card.json\nsurfaces:\n  - surface: REST\n    endpoint: https://www.lacuna.fm/api/v1/music/generations\n    auth_required: true\n  - surface: MCP (Streamable HTTP)\n    endpoint: https://www.lacuna.fm/mcp\n    auth_required: partial\n    note: initialize and tools/list answer anonymously; tools/call requires a credential.\n\
  \  - surface: A2A (JSON-RPC)\n    endpoint: https://www.lacuna.fm/a2a\n    auth_required: true\n    note: Anonymous POST observed returning 401 authentication_error / invalid_api_key.\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n    - url: https://www.lacuna.fm/auth.md\n      http_status: 200\n    - url: https://www.lacuna.fm/.well-known/oauth-authorization-server\n      http_status: 200\n    - url: https://www.lacuna.fm/.well-known/oauth-protected-resource\n      http_status: 200\n    - url: https://www.lacuna.fm/api/openapi.json\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/authentication/lacuna-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Music
- Music Generation
- AI Song Generator
- AI Lyrics Generator
- Audio
- MIDI
- Songwriting
- Generative AI
- MCP Server
- AgentSkill
- A2A
- Developer Tools
---
