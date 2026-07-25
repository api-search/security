---
api_key_in: []
api_specs:
- filename: midpage-opinions-api-openapi.yml
  format: yaml
  label: Midpage Opinions API
  slug: midpage-opinions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-opinions-api-openapi.yml
- filename: midpage-search-api-openapi.yml
  format: yaml
  label: Midpage Search API
  slug: midpage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-search-api-openapi.yml
- filename: midpage-user-api-openapi.yml
  format: yaml
  label: Midpage User API
  slug: midpage-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Midpage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Midpage secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Midpage
provider_slug: midpage
scheme_count: 1
schemes:
- description: API key authentication. Get your API key from the Midpage Developer Portal at https://app.midpage.ai/developers
  name: apiKey
  scheme: bearer
  sources:
  - openapi/midpage-openapi.yml
  type: http
slug: midpage-authentication
source_filename: midpage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/midpage-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: API key authentication. Get your API key from the Midpage Developer Portal at\n    https://app.midpage.ai/developers\n  sources:\n  - openapi/midpage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/authentication/midpage-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal
- Case Law
- Legal Research
- Search
- AI
---
