---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: painspotter-ai-blog-api-openapi.yml
  format: yaml
  label: Pain Spotter Blog API
  slug: painspotter-ai-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/painspotter-ai/openapi/painspotter-ai-blog-api-openapi.yml
- filename: painspotter-ai-opportunities-api-openapi.yml
  format: yaml
  label: Pain Spotter Opportunities API
  slug: painspotter-ai-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/painspotter-ai/openapi/painspotter-ai-opportunities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pain Spotter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pain Spotter secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pain Spotter
provider_slug: painspotter-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/painspotter-ai-openapi.json
  type: apiKey
slug: painspotter-ai-authentication
source_filename: painspotter-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/painspotter-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/painspotter-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/painspotter-ai/authentication/painspotter-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Analytics
- Market Research
- Business Intelligence
- Startup Tools
---
