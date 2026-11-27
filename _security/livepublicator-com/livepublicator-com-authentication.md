---
anonymous_access: false
api_key_in: []
api_specs:
- filename: livepublicator-com-credits-api-openapi.yml
  format: yaml
  label: LivePublicator Credits API
  slug: livepublicator-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livepublicator-com/openapi/livepublicator-com-credits-api-openapi.yml
- filename: livepublicator-com-releases-api-openapi.yml
  format: yaml
  label: LivePublicator Releases API
  slug: livepublicator-com-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livepublicator-com/openapi/livepublicator-com-releases-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LivePublicator Authentication
name_suffix: Authentication
oauth_flows: []
overview: LivePublicator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LivePublicator
provider_slug: livepublicator-com
scheme_count: 1
schemes:
- description: Your API key from the account area (starts with lp_live_).
  name: bearer
  scheme: bearer
  sources:
  - openapi/livepublicator-com-openapi.json
  type: http
slug: livepublicator-com-authentication
source_filename: livepublicator-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/livepublicator-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Your API key from the account area (starts with lp_live_).\n  sources:\n  - openapi/livepublicator-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/livepublicator-com/authentication/livepublicator-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Press Releases
- AI‑ready publishing
- Company newsroom
- Content Publishing
---
