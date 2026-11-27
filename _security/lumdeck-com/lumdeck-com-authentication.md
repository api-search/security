---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumdeck-com-guest-api-openapi.yml
  format: yaml
  label: Lumdeck Guest API
  slug: lumdeck-com-guest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumdeck-com/openapi/lumdeck-com-guest-api-openapi.yml
- filename: lumdeck-com-presentations-api-openapi.yml
  format: yaml
  label: Lumdeck Presentations API
  slug: lumdeck-com-presentations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumdeck-com/openapi/lumdeck-com-presentations-api-openapi.yml
- filename: lumdeck-com-shares-api-openapi.yml
  format: yaml
  label: Lumdeck Shares API
  slug: lumdeck-com-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumdeck-com/openapi/lumdeck-com-shares-api-openapi.yml
- filename: lumdeck-com-workspace-api-openapi.yml
  format: yaml
  label: Lumdeck Workspace API
  slug: lumdeck-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumdeck-com/openapi/lumdeck-com-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lumdeck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumdeck secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumdeck
provider_slug: lumdeck-com
scheme_count: 1
schemes:
- description: A Lumdeck API key (prs_…).
  name: apiKey
  scheme: bearer
  sources:
  - openapi/lumdeck-com-openapi.json
  type: http
slug: lumdeck-com-authentication
source_filename: lumdeck-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lumdeck-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: A Lumdeck API key (prs_…).\n  sources:\n  - openapi/lumdeck-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lumdeck-com/authentication/lumdeck-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Presentation
- Sharing
- Web Service
- Video
---
