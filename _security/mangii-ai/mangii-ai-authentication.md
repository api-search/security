---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mangii-ai-billing-api-openapi.yml
  format: yaml
  label: Mangii Billing API
  slug: mangii-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mangii-ai/openapi/mangii-ai-billing-api-openapi.yml
- filename: mangii-ai-catalog-api-openapi.yml
  format: yaml
  label: Mangii Catalog API
  slug: mangii-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mangii-ai/openapi/mangii-ai-catalog-api-openapi.yml
- filename: mangii-ai-images-api-openapi.yml
  format: yaml
  label: Mangii Images API
  slug: mangii-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mangii-ai/openapi/mangii-ai-images-api-openapi.yml
- filename: mangii-ai-jobs-api-openapi.yml
  format: yaml
  label: Mangii Jobs API
  slug: mangii-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mangii-ai/openapi/mangii-ai-jobs-api-openapi.yml
- filename: mangii-ai-stories-api-openapi.yml
  format: yaml
  label: Mangii Stories API
  slug: mangii-ai-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mangii-ai/openapi/mangii-ai-stories-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mangii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mangii secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mangii
provider_slug: mangii-ai
scheme_count: 1
schemes:
- bearerFormat: mangii_sk_
  description: API key mangii_sk_<32 bytes base62>
  name: mangiiKey
  scheme: bearer
  sources:
  - openapi/mangii-ai-openapi.json
  type: http
slug: mangii-ai-authentication
source_filename: mangii-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mangii-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: mangiiKey\n  type: http\n  scheme: bearer\n  bearerFormat: mangii_sk_\n  description: API key mangii_sk_<32 bytes base62>\n  sources:\n  - openapi/mangii-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mangii-ai/authentication/mangii-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Manga
- Generation
- Creative
- Platform
---
