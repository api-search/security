---
api_key_in:
- header
api_specs:
- filename: reonic-openapi-original.json
  format: json
  label: Reonic REST API v3
  slug: reonic-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonic/refs/heads/main/openapi/reonic-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Reonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reonic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reonic
provider_slug: reonic
scheme_count: 1
schemes:
- in: header
  name: X-Authorization
  parameter: X-Authorization
  sources:
  - openapi/reonic-openapi-original.json
  type: apiKey
slug: reonic-authentication
source_filename: reonic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/reonic-openapi-original.json\ndocs: https://api.reonic.de/rest/v3/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  key_prefix: rnc_v3_\n  key_access_levels: [read-only, read-and-write]\n  notes: >-\n    Every request must include the full API key (including the rnc_v3_ prefix) in the\n    X-Authorization header. Keys are issued in the Reonic Portal (Settings > Integrations).\n    Read-only keys receive 403 on write (POST) endpoints. v2 keys do not work on v3.\n    OIDC Single Sign-On is offered for app login only, not for API access.\nschemes:\n- name: X-Authorization\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  sources:\n  - openapi/reonic-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reonic/refs/heads/main/authentication/reonic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Climate Energy
- Solar
- Renewable Energy
- Photovoltaic
- Heat Pumps
- Installer Software
- SaaS
- CRM
- Project Management
---
