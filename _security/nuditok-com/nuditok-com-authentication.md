---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuditok-com-agents-api-openapi.yml
  format: yaml
  label: NudiTok Agents API
  slug: nuditok-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuditok-com/openapi/nuditok-com-agents-api-openapi.yml
- filename: nuditok-com-tags-api-openapi.yml
  format: yaml
  label: NudiTok Tags API
  slug: nuditok-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuditok-com/openapi/nuditok-com-tags-api-openapi.yml
- filename: nuditok-com-users-api-openapi.yml
  format: yaml
  label: NudiTok Users API
  slug: nuditok-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuditok-com/openapi/nuditok-com-users-api-openapi.yml
- filename: nuditok-com-videos-api-openapi.yml
  format: yaml
  label: NudiTok Videos API
  slug: nuditok-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuditok-com/openapi/nuditok-com-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NudiTok Authentication
name_suffix: Authentication
oauth_flows: []
overview: NudiTok secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NudiTok
provider_slug: nuditok-com
scheme_count: 1
schemes:
- bearerFormat: ntok_<hex>
  description: Personal Access Token with scope videos:write or admin:*
  name: BearerPAT
  scheme: bearer
  sources:
  - openapi/nuditok-com-openapi.json
  type: http
slug: nuditok-com-authentication
source_filename: nuditok-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nuditok-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerPAT\n  type: http\n  scheme: bearer\n  bearerFormat: ntok_<hex>\n  description: Personal Access Token with scope videos:write or admin:*\n  sources:\n  - openapi/nuditok-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nuditok-com/authentication/nuditok-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Adult Content
- NSFW
---
