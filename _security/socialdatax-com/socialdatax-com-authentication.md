---
anonymous_access: false
api_key_in: []
api_specs:
- filename: socialdatax-com-default-api-openapi.yml
  format: yaml
  label: socialdatax-com 互动列表 API
  slug: socialdatax-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdatax-com/openapi/socialdatax-com-default-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Socialdatax Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: socialdatax-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: socialdatax-com
provider_slug: socialdatax-com
scheme_count: 1
schemes:
- description: 'Authorization: Bearer <API_KEY>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/socialdatax-com-openapi-full.json
  - openapi/socialdatax-com-openapi.json
  type: http
slug: socialdatax-com-authentication
source_filename: socialdatax-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/socialdatax-com-openapi-full.json, openapi/socialdatax-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <API_KEY>'\n  sources:\n  - openapi/socialdatax-com-openapi-full.json\n  - openapi/socialdatax-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/socialdatax-com/authentication/socialdatax-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Social Media
- Data Integration
- AI
- API
---
