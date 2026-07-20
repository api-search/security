---
api_key_in: []
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Clockwork Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clockwork Labs secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clockwork Labs
provider_slug: clockwork-labs
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer JWT in the Authorization header. Accepted on write/privileged HTTP endpoints (publish, delete, logs, names, reducer calls, SQL) and on the subscription WebSocket. When present, the response echoes spacetime-identity and spacetime-identity-token headers.
  name: bearerAuth
  scheme: bearer
  type: http
- description: 'SpacetimeAuth (beta) is the first-party OIDC identity provider. Third-party OIDC providers are also supported and documented: Auth0, Clerk, and Steam Session Ticket authentication. Any OIDC ID token whose issuer the module trusts can be used as the Bearer token.'
  issuer: https://auth.spacetimedb.com
  name: spacetimeAuth
  openIdConnectUrl: https://spacetimedb.com/.well-known/openid-configuration
  type: openIdConnect
slug: clockwork-labs-authentication
source_filename: clockwork-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://spacetimedb.com/docs/core-concepts/authentication\ndocs: https://spacetimedb.com/docs/core-concepts/authentication\nnote: >-\n  SpacetimeDB has no OpenAPI to derive from; this profile is captured from the documented HTTP API\n  and authentication docs. Authentication is a Bearer JWT presented in the Authorization header.\n  Tokens are OpenID Connect (OIDC) ID tokens whose issuer is trusted by the module. SpacetimeDB\n  can also mint an anonymous identity+token pair (POST /v1/identity) for clients with no external\n  IdP. The public key used to verify tokens is exposed at GET /v1/identity/public-key and via the\n  OIDC discovery document (well-known/clockwork-labs-openid-configuration.json).\nsummary:\n  types: [http, openIdConnect]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oidc_issuer: https://auth.spacetimedb.com\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description:\
  \ >-\n    Bearer JWT in the Authorization header. Accepted on write/privileged HTTP endpoints (publish,\n    delete, logs, names, reducer calls, SQL) and on the subscription WebSocket. When present, the\n    response echoes spacetime-identity and spacetime-identity-token headers.\n- name: spacetimeAuth\n  type: openIdConnect\n  openIdConnectUrl: https://spacetimedb.com/.well-known/openid-configuration\n  issuer: https://auth.spacetimedb.com\n  description: >-\n    SpacetimeAuth (beta) is the first-party OIDC identity provider. Third-party OIDC providers are\n    also supported and documented: Auth0, Clerk, and Steam Session Ticket authentication. Any OIDC\n    ID token whose issuer the module trusts can be used as the Bearer token.\nproviders:\n- name: SpacetimeAuth\n  status: beta\n  docs: https://spacetimedb.com/docs/core-concepts/authentication/spacetimeauth/\n- name: Auth0\n  docs: https://spacetimedb.com/docs/core-concepts/authentication/Auth0\n- name: Clerk\n  docs: https://spacetimedb.com/docs/core-concepts/authentication/Clerk\n\
  - name: Steam Session Ticket\n  docs: https://spacetimedb.com/docs/core-concepts/authentication/spacetimeauth/steam\ntokens:\n  anonymous_identity:\n    endpoint: POST /v1/identity\n    description: Generate a new anonymous identity and long-lived token.\n  websocket_token:\n    endpoint: POST /v1/identity/websocket-token\n    description: >-\n      Generate a short-lived access token (JWT) for use in untrusted contexts, e.g. embedded in a\n      subscription WebSocket URL.\n  verify:\n    endpoint: GET /v1/identity/:identity/verify\n    description: Verify an identity/token pair (204 valid-and-matches, 400 valid-but-mismatch, 401 invalid).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockwork-labs/refs/heads/main/authentication/clockwork-labs-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Company
- Database
- Real-Time
- WebSocket
- Game Backend
- Multiplayer
- Serverless
- WebAssembly
- Developer Tools
- Infrastructure
---
