---
api_key_in:
- header
api_specs:
- filename: workspace-openapi-original.json
  format: json
  label: VSCO Workspace API
  slug: vsco-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vsco/refs/heads/main/openapi/workspace-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vsco Authentication
name_suffix: Authentication
oauth_flows: []
overview: VSCO secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VSCO
provider_slug: vsco
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/workspace-openapi-original.json
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/workspace-openapi-original.json
  type: http
slug: vsco-authentication
source_filename: vsco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/workspace-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/workspace-openapi-original.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/workspace-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vsco/refs/heads/main/authentication/vsco-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Consumer
- Photography
- Photo Editing
- Creative Community
- Studio Management
- SaaS
---
