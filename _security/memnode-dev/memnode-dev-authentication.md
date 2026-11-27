---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: memnode Authentication
name_suffix: Authentication
oauth_flows: []
overview: memnode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: memnode
provider_slug: memnode-dev
scheme_count: 1
schemes:
- bearerFormat: API Token
  description: Hosted Memnode API token.
  name: BearerApiToken
  scheme: bearer
  sources:
  - openapi/memnode-dev-openapi.json
  type: http
slug: memnode-dev-authentication
source_filename: memnode-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/memnode-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  description: Hosted Memnode API token.\n  sources:\n  - openapi/memnode-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/memnode-dev/authentication/memnode-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Memory
- Agents
- Platform
---
