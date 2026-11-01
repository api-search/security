---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tickerlayer-openapi-generated.yml
  format: yaml
  label: TickerLayer API
  slug: tickerlayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerlayer/openapi/_ae-authored/tickerlayer-openapi-generated.yml
auth_types: []
description: TickerLayer uses a single API key for both REST and WebSocket authentication.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tickerlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: TickerLayer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TickerLayer
provider_slug: tickerlayer
scheme_count: 2
schemes:
- evidence: 'Send the key as Use Header x-api-key : <YOUR_API_KEY>'
  header: x-api-key
  how_to_obtain: Get an API key from the Dashboard (sign‑up and reveal the key).
  location: header
  name: x-api-key
  type: apiKey
- evidence: Query parameter ? apiKey = <YOUR_API_KEY>
  how_to_obtain: Get an API key from the Dashboard (sign‑up and reveal the key).
  location: query
  name: apiKey
  type: apiKey
slug: tickerlayer-authentication
source_filename: tickerlayer-authentication.yml
source_heading: Authentication Profile
source_url: https://tickerlayer.com/docs/authentication
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tickerlayer.com/docs/authentication\nsources:\n- https://tickerlayer.com/docs/authentication\n- https://tickerlayer.com/docs/websocket/authentication\n- https://tickerlayer.com/docs/authentication.md\n- https://tickerlayer.com/docs/quickstart\ndescription: TickerLayer uses a single API key for both REST and WebSocket authentication.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Send the key as Use Header x-api-key : <YOUR_API_KEY>'\n  location: header\n  header: x-api-key\n  how_to_obtain: Get an API key from the Dashboard (sign‑up and reveal the key).\n- type: apiKey\n  name: apiKey\n  evidence: Query parameter ? apiKey = <YOUR_API_KEY>\n  location: query\n  how_to_obtain: Get an API key from the Dashboard (sign‑up and reveal the key).\nnote: Both schemes are interchangeable; the header is preferred for REST, while the query parameter is used for WebSocket\
  \ upgrade URLs.\ndocs: https://tickerlayer.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/tickerlayer/authentication/tickerlayer-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Market Data
- Real-Time
- Finance
---
