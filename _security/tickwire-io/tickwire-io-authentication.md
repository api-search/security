---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes as published on Tickwire documentation.
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Tickwire Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tickwire declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Tickwire
provider_slug: tickwire-io
scheme_count: 6
schemes:
- evidence: The header forms Tickwire accepts, token kinds, and how to narrow a token's reach.
  header: X-Tickwire-Agent-Key
  how_to_obtain: Created under **AI agents > Keys** in the dashboard.
  location: header
  name: X-Tickwire-Agent-Key
  type: apiKey
- evidence: 'Every request carries a key or token. We accept each of the forms the APIs we''re compatible with use, so existing clients work unchanged:'
  header: Authorization
  how_to_obtain: Created as API keys (`tw_live_`, `tw_ro_`) or Agent keys (`twag_`) in the dashboard.
  location: header
  name: Authorization Bearer
  type: http-bearer
- evidence: '`X-API-Key` header | `X-API-Key: <key>` | The `/v1` API and terminal routes'
  header: X-API-Key
  how_to_obtain: Created under **API keys** in the dashboard.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: '`auth-token` header | `auth-token: <token>` | The `/users/current/…` REST API'
  header: auth-token
  how_to_obtain: Derived as a scoped token from an API key for browser pages.
  location: header
  name: auth-token
  type: apiKey
- evidence: Query parameter | `?auth-token=<token>` or `?api_key=<key>` | WebSocket and socket.io connections only, for clients that can't set headers (browsers)
  header: auth-token
  how_to_obtain: Derived as a scoped token from an API key for browser pages.
  location: query
  name: auth-token (query)
  type: apiKey
- evidence: Query parameter | `?auth-token=<token>` or `?api_key=<key>` | WebSocket and socket.io connections only, for clients that can't set headers (browsers)
  header: api_key
  how_to_obtain: Derived as a scoped token from an API key for browser pages.
  location: query
  name: api_key (query)
  type: apiKey
slug: tickwire-io-authentication
source_filename: tickwire-io-authentication.yml
source_heading: Authentication Profile
source_url: https://tickwire.io/docs/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tickwire.io/docs/authentication.md\nsources:\n- https://tickwire.io/docs/authentication.md\n- https://tickwire.io/docs/reference/oauth.md\n- https://tickwire.io/blog/keep-trading-api-keys-safe.md\n- https://tickwire.io/docs/errors/api_key_expired.md\ndescription: Authentication schemes as published on Tickwire documentation.\nschemes:\n- type: apiKey\n  name: X-Tickwire-Agent-Key\n  evidence: The header forms Tickwire accepts, token kinds, and how to narrow a token's reach.\n  location: header\n  header: X-Tickwire-Agent-Key\n  how_to_obtain: Created under **AI agents > Keys** in the dashboard.\n- type: http-bearer\n  name: Authorization Bearer\n  evidence: 'Every request carries a key or token. We accept each of the forms the APIs we''re compatible with use, so existing clients work unchanged:'\n  location: header\n  header: Authorization\n  how_to_obtain: Created as API\
  \ keys (`tw_live_`, `tw_ro_`) or Agent keys (`twag_`) in the dashboard.\n- type: apiKey\n  name: X-API-Key\n  evidence: '`X-API-Key` header | `X-API-Key: <key>` | The `/v1` API and terminal routes'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Created under **API keys** in the dashboard.\n- type: apiKey\n  name: auth-token\n  evidence: '`auth-token` header | `auth-token: <token>` | The `/users/current/…` REST API'\n  location: header\n  header: auth-token\n  how_to_obtain: Derived as a scoped token from an API key for browser pages.\n- type: apiKey\n  name: auth-token (query)\n  evidence: Query parameter | `?auth-token=<token>` or `?api_key=<key>` | WebSocket and socket.io connections only, for clients that can't set\n    headers (browsers)\n  location: query\n  header: auth-token\n  how_to_obtain: Derived as a scoped token from an API key for browser pages.\n- type: apiKey\n  name: api_key (query)\n  evidence: Query parameter | `?auth-token=<token>` or `?api_key=<key>` |\
  \ WebSocket and socket.io connections only, for clients that can't set\n    headers (browsers)\n  location: query\n  header: api_key\n  how_to_obtain: Derived as a scoped token from an API key for browser pages.\nnote: OAuth flows are not described with token or authorize URLs; all OAuth endpoints require an X-API-Key header as shown in the OAuth reference\n  pages.\ndocs: https://tickwire.io/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/tickwire-io/authentication/tickwire-io-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Finance
- Trading
- API
- MetaTrader
---
