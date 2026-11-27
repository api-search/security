---
anonymous_access: false
api_key_in: []
api_specs:
- filename: desaira-com-agents-api-openapi.yml
  format: yaml
  label: DesAira Agents API
  slug: desaira-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-agents-api-openapi.yml
- filename: desaira-com-tags-api-openapi.yml
  format: yaml
  label: DesAira Tags API
  slug: desaira-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-tags-api-openapi.yml
- filename: desaira-com-users-api-openapi.yml
  format: yaml
  label: DesAira Users API
  slug: desaira-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-users-api-openapi.yml
- filename: desaira-com-videos-api-openapi.yml
  format: yaml
  label: DesAira Videos API
  slug: desaira-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DesAira Authentication
name_suffix: Authentication
oauth_flows: []
overview: DesAira secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DesAira
provider_slug: desaira-com
scheme_count: 1
schemes:
- bearerFormat: ntok_<hex>
  description: Personal Access Token with scope videos:write or admin:*
  name: BearerPAT
  scheme: bearer
  sources:
  - openapi/desaira-com-openapi.json
  type: http
slug: desaira-com-authentication
source_filename: desaira-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/desaira-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerPAT\n  type: http\n  scheme: bearer\n  bearerFormat: ntok_<hex>\n  description: Personal Access Token with scope videos:write or admin:*\n  sources:\n  - openapi/desaira-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/desaira-com/authentication/desaira-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Adult
- Artificial Intelligence
- Pornography
- Video
- Platform
---
