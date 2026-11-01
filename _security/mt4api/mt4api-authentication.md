---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Noble Minds Media (FxSocket) APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mt4Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noble Minds Media declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Noble Minds Media
provider_slug: mt4api
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
slug: mt4api-authentication
source_filename: mt4api-authentication.yml
source_heading: Authentication Profile
source_url: https://fxsocket.com/docs/mt5/authentication
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fxsocket.com/docs/mt5/authentication\nsources:\n- https://fxsocket.com/docs/mt5/authentication\n- https://fxsocket.com/docs/mt4/authentication\n- https://fxsocket.com/docs/mcp\ndescription: Authentication schemes for Noble Minds Media (FxSocket) APIs\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every FxSocket API request is authenticated with a per-user API key, passed as an X-API-Key header, or as an api_key query parameter\n    for clients (like WebSocket) that can't set headers.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Copy it from the dashboard's API Key page.\n- type: apiKey\n  name: api_key\n  evidence: Every FxSocket API request is authenticated with a per-user API key, passed as an X-API-Key header, or as an api_key query parameter\n    for clients (like WebSocket) that can't set headers.\n  location: query\n  how_to_obtain: Copy it\
  \ from the dashboard's API Key page.\nnote: No OAuth2, Bearer, or other authentication schemes are documented.\ndocs: https://fxsocket.com/docs/mt5/authentication\n"
source_yaml_url: https://artifacts.apis.io/mt4api/authentication/mt4api-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Trading
- API
- MetaTrader
- Data
---
