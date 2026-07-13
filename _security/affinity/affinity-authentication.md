---
api_key_in: []
api_specs:
- filename: affinity-v2-openapi.yml
  format: yaml
  label: Affinity API V2
  slug: affinity-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-v2-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Affinity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affinity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Affinity
provider_slug: affinity
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/affinity-v2-openapi.yml
  type: http
slug: affinity-authentication
source_filename: affinity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/affinity-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/affinity-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/authentication/affinity-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Relationship Intelligence
- Private Equity
- Venture Capital
- Contacts
- Organizations
- Opportunities
- Deal Management
---
