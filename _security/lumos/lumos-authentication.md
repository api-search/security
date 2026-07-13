---
api_key_in: []
api_specs:
- filename: lumos-openapi.yml
  format: yaml
  label: Lumos REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lumos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumos secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumos
provider_slug: lumos
scheme_count: 1
schemes:
- bearerFormat: Lumos API key (lsk_ prefix)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lumos-openapi.yml
  type: http
slug: lumos-authentication
source_filename: lumos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lumos-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Lumos API key (lsk_ prefix)\n  sources:\n  - openapi/lumos-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/authentication/lumos-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
---
