---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gmaps-dev-attributions-api-openapi.yml
  format: yaml
  label: gmaps.dev Attributions API
  slug: gmaps-dev-attributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-attributions-api-openapi.yml
- filename: gmaps-dev-collections-api-openapi.yml
  format: yaml
  label: gmaps.dev Collections API
  slug: gmaps-dev-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-collections-api-openapi.yml
- filename: gmaps-dev-coverage-api-openapi.yml
  format: yaml
  label: gmaps.dev Coverage API
  slug: gmaps-dev-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-coverage-api-openapi.yml
- filename: gmaps-dev-exports-api-openapi.yml
  format: yaml
  label: gmaps.dev Exports API
  slug: gmaps-dev-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-exports-api-openapi.yml
- filename: gmaps-dev-places-api-openapi.yml
  format: yaml
  label: gmaps.dev Places API
  slug: gmaps-dev-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-places-api-openapi.yml
- filename: gmaps-dev-usage-api-openapi.yml
  format: yaml
  label: gmaps.dev Usage API
  slug: gmaps-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-usage-api-openapi.yml
- filename: gmaps-dev-webhooks-api-openapi.yml
  format: yaml
  label: gmaps.dev Webhooks API
  slug: gmaps-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmaps-dev/openapi/gmaps-dev-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: gmaps.dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: gmaps.dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: gmaps.dev
provider_slug: gmaps-dev
scheme_count: 1
schemes:
- description: 'Send your API key as "Authorization: Bearer gm_…".'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/gmaps-dev-openapi.json
  type: http
slug: gmaps-dev-authentication
source_filename: gmaps-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gmaps-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Send your API key as \"Authorization: Bearer gm_…\".'\n  sources:\n  - openapi/gmaps-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gmaps-dev/authentication/gmaps-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Leads
- Location Data
- Business-API
- Google-Maps-Data
- AI Agents
---
