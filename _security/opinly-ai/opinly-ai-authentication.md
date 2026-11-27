---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opinly-ai-content-api-openapi.yml
  format: yaml
  label: Opinly Content API
  slug: opinly-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opinly-ai/openapi/opinly-ai-content-api-openapi.yml
- filename: opinly-ai-events-api-openapi.yml
  format: yaml
  label: Opinly Events API
  slug: opinly-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opinly-ai/openapi/opinly-ai-events-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Opinly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opinly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opinly
provider_slug: opinly-ai
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/opinly-ai-openapi.yml
  type: http
slug: opinly-ai-authentication
source_filename: opinly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/opinly-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/opinly-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/opinly-ai/authentication/opinly-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SEO
- Artificial Intelligence
- Marketing
- Automation
---
