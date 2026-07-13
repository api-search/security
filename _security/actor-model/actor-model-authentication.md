---
api_key_in: []
api_specs:
- filename: actor-model.json
  format: json
  label: Actor Model API
  slug: actor-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/openapi/actor-model.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Actor Model Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actor Model secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Actor Model
provider_slug: actor-model
scheme_count: 1
schemes:
- description: Bearer token for actor system management API access
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/actor-model.json
  type: http
slug: actor-model-authentication
source_filename: actor-model-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/actor-model.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for actor system management API access\n  sources:\n  - openapi/actor-model.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/authentication/actor-model-authentication.yml
summary_line: http · 1 scheme
tags:
- Actor Model
- Concurrency
- Distributed Systems
---
