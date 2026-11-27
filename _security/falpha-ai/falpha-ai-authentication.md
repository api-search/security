---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: falpha-ai-account-api-openapi.yml
  format: yaml
  label: fAlpha Account API
  slug: falpha-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-account-api-openapi.yml
- filename: falpha-ai-discovery-api-openapi.yml
  format: yaml
  label: fAlpha Discovery API
  slug: falpha-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-discovery-api-openapi.yml
- filename: falpha-ai-events-api-openapi.yml
  format: yaml
  label: fAlpha Events API
  slug: falpha-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-events-api-openapi.yml
- filename: falpha-ai-health-api-openapi.yml
  format: yaml
  label: fAlpha Health API
  slug: falpha-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-health-api-openapi.yml
- filename: falpha-ai-news-api-openapi.yml
  format: yaml
  label: fAlpha News API
  slug: falpha-ai-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-news-api-openapi.yml
- filename: falpha-ai-signals-api-openapi.yml
  format: yaml
  label: fAlpha Signals API
  slug: falpha-ai-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falpha-ai/openapi/falpha-ai-signals-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: fAlpha Authentication
name_suffix: Authentication
oauth_flows: []
overview: fAlpha secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: fAlpha
provider_slug: falpha-ai
scheme_count: 2
schemes:
- in: query
  name: APIKeyQuery
  parameter: api_key
  sources:
  - openapi/falpha-ai-openapi.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/falpha-ai-openapi.json
  type: apiKey
slug: falpha-ai-authentication
source_filename: falpha-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/falpha-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: APIKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/falpha-ai-openapi.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/falpha-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/falpha-ai/authentication/falpha-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Finance
- Artificial Intelligence
- Trading
- Validation
- Analytics
---
