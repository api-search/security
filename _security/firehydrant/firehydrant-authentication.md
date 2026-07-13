---
api_key_in: []
api_specs:
- filename: firehydrant-openapi.yml
  format: yaml
  label: FireHydrant
  slug: firehydrant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Firehydrant Authentication
name_suffix: Authentication
oauth_flows: []
overview: FireHydrant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FireHydrant
provider_slug: firehydrant
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/firehydrant-openapi.yml
  type: http
slug: firehydrant-authentication
source_filename: firehydrant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/firehydrant-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/firehydrant-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/authentication/firehydrant-authentication.yml
summary_line: http · 1 scheme
tags:
- AIOps
- Incident Management
---
