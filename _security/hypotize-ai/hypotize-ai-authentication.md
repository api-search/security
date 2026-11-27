---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hypotize-ai-comments-api-openapi.yml
  format: yaml
  label: Hypotize Comments API
  slug: hypotize-ai-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypotize-ai/openapi/hypotize-ai-comments-api-openapi.yml
- filename: hypotize-ai-experiments-api-openapi.yml
  format: yaml
  label: Hypotize Experiments API
  slug: hypotize-ai-experiments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypotize-ai/openapi/hypotize-ai-experiments-api-openapi.yml
- filename: hypotize-ai-learnings-api-openapi.yml
  format: yaml
  label: Hypotize Learnings API
  slug: hypotize-ai-learnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypotize-ai/openapi/hypotize-ai-learnings-api-openapi.yml
- filename: hypotize-ai-projects-api-openapi.yml
  format: yaml
  label: Hypotize Projects API
  slug: hypotize-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypotize-ai/openapi/hypotize-ai-projects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hypotize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hypotize secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hypotize
provider_slug: hypotize-ai
scheme_count: 1
schemes:
- bearerFormat: hyp_ API key
  description: Personal API key from Settings, API keys.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/hypotize-ai-openapi.json
  type: http
slug: hypotize-ai-authentication
source_filename: hypotize-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/hypotize-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: hyp_ API key\n  description: Personal API key from Settings, API keys.\n  sources:\n  - openapi/hypotize-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hypotize-ai/authentication/hypotize-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Growth
- Artificial Intelligence
- Automation
- Experimentation
- Platform
- Company
---
