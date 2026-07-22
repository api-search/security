---
api_key_in: []
api_specs:
- filename: permutive-openapi.yml
  format: yaml
  label: Permutive API
  slug: permutive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Permutive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Permutive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Permutive
provider_slug: permutive
scheme_count: 1
schemes:
- description: Permutive workspace API key supplied as a bearer token. See https://developer.permutive.com/api/authentication for the exact header and key-provisioning details.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/permutive-openapi.yml
  type: http
slug: permutive-authentication
source_filename: permutive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/permutive-openapi.yml\ndocs: https://developer.permutive.com/api/authentication\nnotes: >-\n  Permutive APIs authenticate with a workspace-scoped API key. Cohorts, imports\n  and admin operations are authorized against the workspace that owns the key.\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: Permutive workspace API key supplied as a bearer token. See https://developer.permutive.com/api/authentication\n    for the exact header and key-provisioning details.\n  sources:\n  - openapi/permutive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/authentication/permutive-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Publishing
- Advertising
- AdTech
- MarTech
- Audience
- Data Collaboration
- Data Management Platform
- Contextual
- Identity
---
