---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tunova-ai-generation-api-openapi.yml
  format: yaml
  label: tunova-ai Generation API
  slug: tunova-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tunova-ai/openapi/tunova-ai-generation-api-openapi.yml
- filename: tunova-ai-jobs-api-openapi.yml
  format: yaml
  label: tunova-ai Jobs API
  slug: tunova-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tunova-ai/openapi/tunova-ai-jobs-api-openapi.yml
- filename: tunova-ai-utility-api-openapi.yml
  format: yaml
  label: tunova-ai Utility API
  slug: tunova-ai-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tunova-ai/openapi/tunova-ai-utility-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tunova Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: tunova-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: tunova-ai
provider_slug: tunova-ai
scheme_count: 1
schemes:
- description: Per-customer key, e.g. sk_live_...
  in: header
  name: X-API-Key
  official: true
  type: apiKey
slug: tunova-ai-authentication
source_filename: tunova-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://api.tunova.ai/.well-known/auth.md\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: Per-customer key, e.g. sk_live_...\n    official: true"
source_yaml_url: https://artifacts.apis.io/tunova-ai/authentication/tunova-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Music
- Audio
- Suno
- TokenizedAPI
- REST
- MCP
---
