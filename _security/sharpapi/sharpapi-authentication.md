---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sharpapi-account-api-openapi.yml
  format: yaml
  label: SharpAPI Account API
  slug: sharpapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-account-api-openapi.yml
- filename: sharpapi-betting-splits-api-openapi.yml
  format: yaml
  label: SharpAPI Betting Splits API
  slug: sharpapi-betting-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-betting-splits-api-openapi.yml
- filename: sharpapi-deep-links-api-openapi.yml
  format: yaml
  label: SharpAPI Deep Links API
  slug: sharpapi-deep-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-deep-links-api-openapi.yml
- filename: sharpapi-events-api-openapi.yml
  format: yaml
  label: SharpAPI Events API
  slug: sharpapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-events-api-openapi.yml
- filename: sharpapi-futures-api-openapi.yml
  format: yaml
  label: SharpAPI Futures API
  slug: sharpapi-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-futures-api-openapi.yml
- filename: sharpapi-game-state-api-openapi.yml
  format: yaml
  label: SharpAPI Game State API
  slug: sharpapi-game-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-game-state-api-openapi.yml
- filename: sharpapi-health-api-openapi.yml
  format: yaml
  label: SharpAPI Health API
  slug: sharpapi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-health-api-openapi.yml
- filename: sharpapi-odds-api-openapi.yml
  format: yaml
  label: SharpAPI Odds API
  slug: sharpapi-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-odds-api-openapi.yml
- filename: sharpapi-opportunities-api-openapi.yml
  format: yaml
  label: SharpAPI Opportunities API
  slug: sharpapi-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-opportunities-api-openapi.yml
- filename: sharpapi-reference-data-api-openapi.yml
  format: yaml
  label: SharpAPI Reference Data API
  slug: sharpapi-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-reference-data-api-openapi.yml
- filename: sharpapi-streaming-api-openapi.yml
  format: yaml
  label: SharpAPI Streaming API
  slug: sharpapi-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-streaming-api-openapi.yml
auth_types: []
description: 'SharpAPI supports three authentication methods: X-API-Key header, Authorization Bearer header, and query parameter.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Sharpapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SharpAPI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: SharpAPI
provider_slug: sharpapi
scheme_count: 3
schemes:
- evidence: The most secure method for server-side applications.
  header: X-API-Key
  how_to_obtain: Your API key is displayed on the main dashboard after signing up.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Standard OAuth-style bearer token format.
  header: Authorization
  how_to_obtain: Your API key is displayed on the main dashboard after signing up.
  location: header
  name: Authorization
  type: http-bearer
- evidence: Useful for SSE streaming in browsers where you cannot set custom headers.
  how_to_obtain: Your API key is displayed on the main dashboard after signing up.
  location: query
  name: api_key
  type: apiKey
slug: sharpapi-authentication
source_filename: sharpapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sharpapi.io/en/authentication/
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sharpapi.io/en/authentication/\nsources:\n- https://docs.sharpapi.io/en/authentication/\n- https://docs.sharpapi.io/en/authentication/\n- https://docs.sharpapi.io/es/authentication/\n- https://docs.sharpapi.io/pt-BR/authentication/\ndescription: 'SharpAPI supports three authentication methods: X-API-Key header, Authorization Bearer header, and query parameter.'\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: The most secure method for server-side applications.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Your API key is displayed on the main dashboard after signing up.\n- type: http-bearer\n  name: Authorization\n  evidence: Standard OAuth-style bearer token format.\n  location: header\n  header: Authorization\n  how_to_obtain: Your API key is displayed on the main dashboard after signing up.\n- type: apiKey\n  name: api_key\n  evidence: Useful\
  \ for SSE streaming in browsers where you cannot set custom headers.\n  location: query\n  how_to_obtain: Your API key is displayed on the main dashboard after signing up.\ndocs: https://docs.sharpapi.io/en/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/authentication/sharpapi-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Sports Betting
- Real-Time Data
- Gambling
---
