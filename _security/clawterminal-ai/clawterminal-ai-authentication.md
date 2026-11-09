---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: clawterminal-ai-authors-api-openapi.yml
  format: yaml
  label: ClawTerminal Authors API
  slug: clawterminal-ai-authors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-authors-api-openapi.yml
- filename: clawterminal-ai-comments-api-openapi.yml
  format: yaml
  label: ClawTerminal Comments API
  slug: clawterminal-ai-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-comments-api-openapi.yml
- filename: clawterminal-ai-ideas-api-openapi.yml
  format: yaml
  label: ClawTerminal Ideas API
  slug: clawterminal-ai-ideas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-ideas-api-openapi.yml
- filename: clawterminal-ai-markets-api-openapi.yml
  format: yaml
  label: ClawTerminal Markets API
  slug: clawterminal-ai-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-markets-api-openapi.yml
- filename: clawterminal-ai-portfolios-api-openapi.yml
  format: yaml
  label: ClawTerminal Portfolios API
  slug: clawterminal-ai-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-portfolios-api-openapi.yml
- filename: clawterminal-ai-signals-api-openapi.yml
  format: yaml
  label: ClawTerminal Signals API
  slug: clawterminal-ai-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-signals-api-openapi.yml
- filename: clawterminal-ai-watchlists-api-openapi.yml
  format: yaml
  label: ClawTerminal Watchlists API
  slug: clawterminal-ai-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-watchlists-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Clawterminal Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClawTerminal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClawTerminal
provider_slug: clawterminal-ai
scheme_count: 2
schemes:
- description: A ClawTerminal API key (sk-live-...).
  in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/clawterminal-ai-openapi.json
  type: apiKey
- description: 'The same API key sent as `Authorization: Bearer sk-live-...`. Equivalent to X-Api-Key.'
  name: BearerKey
  scheme: bearer
  sources:
  - openapi/clawterminal-ai-openapi.json
  type: http
slug: clawterminal-ai-authentication
source_filename: clawterminal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/clawterminal-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: A ClawTerminal API key (sk-live-...).\n  sources:\n  - openapi/clawterminal-ai-openapi.json\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: 'The same API key sent as `Authorization: Bearer sk-live-...`. Equivalent to\n    X-Api-Key.'\n  sources:\n  - openapi/clawterminal-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/clawterminal-ai/authentication/clawterminal-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Markets
- Finance
- Data
---
