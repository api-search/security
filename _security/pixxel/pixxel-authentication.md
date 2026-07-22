---
api_key_in:
- header
api_specs:
- filename: pixxel-openapi-original.json
  format: json
  label: Pixxel API (stargate)
  slug: pixxel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pixxel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixxel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pixxel
provider_slug: pixxel
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  scheme_detail: Bearer Personal Access Token
  sources:
  - openapi/pixxel-openapi-original.json
  type: apiKey
slug: pixxel-authentication
source_filename: pixxel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pixxel-openapi-original.json\ndocs: https://docs.pixxel.space/developer/gettingstarted/authentication.md\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: Personal Access Token (bearer)\n  header: 'Authorization: Bearer <PERSONAL_ACCESS_TOKEN>'\n  scoped_by:\n  - organization\n  - project\n  - role\n  provisioning: Aurora platform -> Settings -> Personal Access Tokens (name, roles, project access, expiry).\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_detail: Bearer Personal Access Token\n  sources:\n  - openapi/pixxel-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/authentication/pixxel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Satellite Imagery
- Earth Observation
- Hyperspectral
- Geospatial
- Remote Sensing
- Analytics
- STAC
---
