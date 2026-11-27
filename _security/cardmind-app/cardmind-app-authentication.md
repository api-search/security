---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cardmind-app-openapi-generated.yml
  format: yaml
  label: CardMind API
  slug: cardmind-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cardmind-app/openapi/_ae-authored/cardmind-app-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CardMind Authentication
name_suffix: Authentication
oauth_flows: []
overview: CardMind declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CardMind
provider_slug: cardmind-app
scheme_count: 2
schemes:
- description: Internal secret header for fleet projects, bypasses rate limits. Not for external developers.
  name: X-Internal-Secret
  type: header
- bearerFormat: JWT
  description: Standard Bearer token in Authorization header. API keys prefixed with cm_live_.
  scheme: bearer
  type: http
slug: cardmind-app-authentication
source_filename: cardmind-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://api.cardmind.app/docs/authentication\nschemes:\n  - type: header\n    name: X-Internal-Secret\n    description: Internal secret header for fleet projects, bypasses rate limits. Not for external developers.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Standard Bearer token in Authorization header. API keys prefixed with cm_live_.\n"
source_yaml_url: https://artifacts.apis.io/cardmind-app/authentication/cardmind-app-authentication.yml
summary_line: 2 schemes
tags:
- Market Intelligence
- Price Data
- Signals
- Ban Watch
- Deck Intelligence
---
