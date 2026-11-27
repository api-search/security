---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: maxcv-ai-account-api-openapi.yml
  format: yaml
  label: MaxCV Account API
  slug: maxcv-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-account-api-openapi.yml
- filename: maxcv-ai-cv-api-openapi.yml
  format: yaml
  label: MaxCV Cv API
  slug: maxcv-ai-cv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-cv-api-openapi.yml
- filename: maxcv-ai-matches-api-openapi.yml
  format: yaml
  label: MaxCV Matches API
  slug: maxcv-ai-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-matches-api-openapi.yml
- filename: maxcv-ai-render-api-openapi.yml
  format: yaml
  label: MaxCV Render API
  slug: maxcv-ai-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-render-api-openapi.yml
- filename: maxcv-ai-score-api-openapi.yml
  format: yaml
  label: MaxCV Score API
  slug: maxcv-ai-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-score-api-openapi.yml
- filename: maxcv-ai-tailor-api-openapi.yml
  format: yaml
  label: MaxCV Tailor API
  slug: maxcv-ai-tailor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-tailor-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MaxCV Authentication
name_suffix: Authentication
oauth_flows: []
overview: MaxCV secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MaxCV
provider_slug: maxcv-ai
scheme_count: 1
schemes:
- in: cookie
  name: sessionCookie
  parameter: session
  sources:
  - openapi/maxcv-ai-openapi.yml
  type: apiKey
slug: maxcv-ai-authentication
source_filename: maxcv-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/maxcv-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  sources:\n  - openapi/maxcv-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/maxcv-ai/authentication/maxcv-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Resume
- Job Search
- Careers
- Automation
- Company
---
