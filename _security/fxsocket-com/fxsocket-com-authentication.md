---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fxsocket-com-openapi-generated.yml
  format: yaml
  label: FxSocket API
  slug: fxsocket-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fxsocket-com/openapi/_ae-authored/fxsocket-com-openapi-generated.yml
auth_types: []
description: FxSocket API requests are authenticated with a per‑user API key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fxsocket Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: FxSocket declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FxSocket
provider_slug: fxsocket-com
scheme_count: 2
schemes:
- evidence: Every FxSocket API request is authenticated with a per-user API key, passed as an X-API-Key header, or as an api_key query parameter for clients (like WebSocket) that can't set headers.
  header: X-API-Key
  how_to_obtain: Copy it from the dashboard's API Key page.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Every FxSocket API request is authenticated with a per-user API key, passed as an X-API-Key header, or as an api_key query parameter for clients (like WebSocket) that can't set headers.
  how_to_obtain: Copy it from the dashboard's API Key page.
  location: query
  name: api_key
  type: apiKey
slug: fxsocket-com-authentication
source_filename: fxsocket-com-authentication.yml
source_heading: Authentication Profile
source_url: https://fxsocket.com/docs/mt5/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fxsocket.com/docs/mt5/authentication.md\nsources:\n- https://fxsocket.com/docs/mt5/authentication.md\n- https://fxsocket.com/docs/mt4/authentication.md\n- https://fxsocket.com/docs/mt5/authentication\n- https://fxsocket.com/docs/mt4/authentication\ndescription: FxSocket API requests are authenticated with a per‑user API key.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every FxSocket API request is authenticated with a per-user API key, passed as an X-API-Key header, or as an api_key query parameter\n    for clients (like WebSocket) that can't set headers.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Copy it from the dashboard's API Key page.\n- type: apiKey\n  name: api_key\n  evidence: Every FxSocket API request is authenticated with a per-user API key, passed as an X-API-Key header, or as an api_key query parameter\n    for clients (like WebSocket)\
  \ that can't set headers.\n  location: query\n  how_to_obtain: Copy it from the dashboard's API Key page.\nnote: There is no OAuth flow, bearer, or other authentication scheme.\ndocs: https://fxsocket.com/docs/mt5/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/fxsocket-com/authentication/fxsocket-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- FinTech
- Trading
- API
- Cloud
---
