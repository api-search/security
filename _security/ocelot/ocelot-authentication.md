---
api_key_in: []
api_specs:
- filename: ocelot-administration-openapi.yml
  format: yaml
  label: Ocelot Administration API
  slug: ocelot-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocelot/refs/heads/main/openapi/ocelot-administration-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ocelot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ocelot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ocelot
provider_slug: ocelot
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ocelot-administration-openapi.yml
  type: http
slug: ocelot-authentication
source_filename: ocelot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ocelot-administration-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ocelot-administration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocelot/refs/heads/main/authentication/ocelot-authentication.yml
summary_line: http · 1 scheme
tags:
- .NET
- API Gateway
- Microservices
- Open Source
---
