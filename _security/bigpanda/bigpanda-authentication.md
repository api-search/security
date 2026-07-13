---
api_key_in: []
api_specs:
- filename: bigpanda-openapi.yml
  format: yaml
  label: BigPanda
  slug: bigpanda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/openapi/bigpanda-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bigpanda Authentication
name_suffix: Authentication
oauth_flows: []
overview: BigPanda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BigPanda
provider_slug: bigpanda
scheme_count: 1
schemes:
- description: BigPanda API Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bigpanda-openapi.yml
  type: http
slug: bigpanda-authentication
source_filename: bigpanda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bigpanda-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: BigPanda API Bearer token\n  sources:\n  - openapi/bigpanda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/authentication/bigpanda-authentication.yml
summary_line: http · 1 scheme
tags:
- Incidents
- Monitoring
- Platform
---
