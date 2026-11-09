---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bizmoon-ai-read-api-openapi.yml
  format: yaml
  label: Bizmoon Read API
  slug: bizmoon-ai-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizmoon-ai/openapi/bizmoon-ai-read-api-openapi.yml
- filename: bizmoon-ai-write-api-openapi.yml
  format: yaml
  label: Bizmoon Write API
  slug: bizmoon-ai-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizmoon-ai/openapi/bizmoon-ai-write-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bizmoon Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bizmoon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bizmoon
provider_slug: bizmoon-ai
scheme_count: 1
schemes:
- bearerFormat: API Key (bm_sk_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bizmoon-ai-openapi.yml
  type: http
slug: bizmoon-ai-authentication
source_filename: bizmoon-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bizmoon-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key (bm_sk_...)\n  sources:\n  - openapi/bizmoon-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/bizmoon-ai/authentication/bizmoon-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Compliance
- Grants
- Small Business
---
