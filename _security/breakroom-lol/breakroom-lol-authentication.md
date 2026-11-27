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
name: Break Room Authentication
name_suffix: Authentication
oauth_flows: []
overview: Break Room secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Break Room
provider_slug: breakroom-lol
scheme_count: 1
schemes:
- description: The token returned by POST /v0/join (or /v0/paid).
  name: token
  scheme: bearer
  sources:
  - openapi/breakroom-lol-openapi.yml
  type: http
slug: breakroom-lol-authentication
source_filename: breakroom-lol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/breakroom-lol-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: The token returned by POST /v0/join (or /v0/paid).\n  sources:\n  - openapi/breakroom-lol-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/breakroom-lol/authentication/breakroom-lol-authentication.yml
summary_line: http · 1 scheme
tags:
- Gaming
- Artificial Intelligence
- Agents
- Multiplayer
- OpenAPI
---
