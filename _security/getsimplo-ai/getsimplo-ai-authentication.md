---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getsimplo-ai-credits-api-openapi.yml
  format: yaml
  label: Simplo Credits API
  slug: getsimplo-ai-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-credits-api-openapi.yml
- filename: getsimplo-ai-generate-api-openapi.yml
  format: yaml
  label: Simplo Generate API
  slug: getsimplo-ai-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-generate-api-openapi.yml
- filename: getsimplo-ai-openapi-json-api-openapi.yml
  format: yaml
  label: Simplo Openapi.json API
  slug: getsimplo-ai-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-openapi-json-api-openapi.yml
- filename: getsimplo-ai-posts-api-openapi.yml
  format: yaml
  label: Simplo Posts API
  slug: getsimplo-ai-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-posts-api-openapi.yml
- filename: getsimplo-ai-projects-api-openapi.yml
  format: yaml
  label: Simplo Projects API
  slug: getsimplo-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-projects-api-openapi.yml
- filename: getsimplo-ai-uploads-api-openapi.yml
  format: yaml
  label: Simplo Uploads API
  slug: getsimplo-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-uploads-api-openapi.yml
- filename: getsimplo-ai-videos-api-openapi.yml
  format: yaml
  label: Simplo Videos API
  slug: getsimplo-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsimplo-ai/openapi/getsimplo-ai-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Simplo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simplo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simplo
provider_slug: getsimplo-ai
scheme_count: 1
schemes:
- description: smp_live_… key from Settings → API keys
  name: apiKey
  scheme: bearer
  sources:
  - openapi/getsimplo-ai-openapi.json
  type: http
slug: getsimplo-ai-authentication
source_filename: getsimplo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getsimplo-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: smp_live_… key from Settings → API keys\n  sources:\n  - openapi/getsimplo-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getsimplo-ai/authentication/getsimplo-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Social Media
- Automation
- Small Business
---
