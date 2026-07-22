---
api_key_in:
- query
api_specs:
- filename: manage-bgl-openapi.yml
  format: yaml
  label: Jade Diabetes REST API
  slug: jade-diabetes-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manage-bgl/refs/heads/main/openapi/manage-bgl-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Manage Bgl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Manage BGL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Manage BGL
provider_slug: manage-bgl
scheme_count: 1
schemes:
- description: Client login token (varchar 40) obtained from POST /login (or the OAuth-style /get_token.html for sensitive data). Passed as the `token` parameter on every subsequent request. HTTPS/SSL required.
  in: query
  name: clientToken
  parameter: token
  sources:
  - openapi/manage-bgl-openapi.yml
  type: apiKey
slug: manage-bgl-authentication
source_filename: manage-bgl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/manage-bgl-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: clientToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Client login token (varchar 40) obtained from POST /login (or the OAuth-style\n    /get_token.html for sensitive data). Passed as the `token` parameter on every subsequent\n    request. HTTPS/SSL required.\n  sources:\n  - openapi/manage-bgl-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manage-bgl/refs/heads/main/authentication/manage-bgl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Diabetes
- Health
- Healthcare
- Digital Health
- Insulin
- Blood Glucose
- Remote Patient Monitoring
- Telemedicine
- REST API
---
