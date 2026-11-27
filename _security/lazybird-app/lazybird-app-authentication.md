---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: lazybird-app-auth-api-openapi.yml
  format: yaml
  label: Lazybird Auth API
  slug: lazybird-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-auth-api-openapi.yml
- filename: lazybird-app-checkout-api-openapi.yml
  format: yaml
  label: Lazybird Checkout API
  slug: lazybird-app-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-checkout-api-openapi.yml
- filename: lazybird-app-generate-speech-api-openapi.yml
  format: yaml
  label: Lazybird Generate Speech API
  slug: lazybird-app-generate-speech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-generate-speech-api-openapi.yml
- filename: lazybird-app-me-api-openapi.yml
  format: yaml
  label: Lazybird Me API
  slug: lazybird-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-me-api-openapi.yml
- filename: lazybird-app-music-api-openapi.yml
  format: yaml
  label: Lazybird Music API
  slug: lazybird-app-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-music-api-openapi.yml
- filename: lazybird-app-projects-api-openapi.yml
  format: yaml
  label: Lazybird Projects API
  slug: lazybird-app-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-projects-api-openapi.yml
- filename: lazybird-app-status-api-openapi.yml
  format: yaml
  label: Lazybird Status API
  slug: lazybird-app-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-status-api-openapi.yml
- filename: lazybird-app-stock-api-openapi.yml
  format: yaml
  label: Lazybird Stock API
  slug: lazybird-app-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-stock-api-openapi.yml
- filename: lazybird-app-voices-api-openapi.yml
  format: yaml
  label: Lazybird Voices API
  slug: lazybird-app-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazybird-app/openapi/lazybird-app-voices-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Lazybird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lazybird secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lazybird
provider_slug: lazybird-app
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/lazybird-app-openapi.json
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/lazybird-app-openapi.json
  type: apiKey
slug: lazybird-app-authentication
source_filename: lazybird-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lazybird-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/lazybird-app-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/lazybird-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lazybird-app/authentication/lazybird-app-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Voiceover
- Text-to-Speech
- Creator Tools
- Multilingual
---
