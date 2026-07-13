---
api_key_in:
- header
api_specs:
- filename: configure8-openapi.yml
  format: yaml
  label: Configure8 REST API
  slug: idp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Configure8 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Configure8 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Configure8
provider_slug: configure8
scheme_count: 1
schemes:
- description: Bearer/API token issued from the Configure8 UI; passed in the Authorization header
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/configure8-openapi.yml
  type: apiKey
slug: configure8-authentication
source_filename: configure8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/configure8-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer/API token issued from the Configure8 UI; passed in the Authorization header\n  sources:\n  - openapi/configure8-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/authentication/configure8-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Catalog
- Cloud Cost
- Developer Experience
- DevOps
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Service Catalog
- SRE
---
