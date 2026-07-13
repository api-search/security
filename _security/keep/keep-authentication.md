---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Keep REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.keephq.dev/openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Keep Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Keep secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Keep
provider_slug: keep
scheme_count: 3
schemes:
- in: header
  name: API Key
  parameter: X-API-KEY
  sources:
  - openapi/keep-openapi.json
  type: apiKey
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/keep-openapi.json
  type: http
- flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/keep-openapi.json
  type: oauth2
slug: keep-authentication
source_filename: keep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keep-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/keep-openapi.json\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/keep-openapi.json\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/keep-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keep/refs/heads/main/authentication/keep-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- AIOps
- Alerting
- Incident Management
- Observability
- Open Source
- SRE
- Workflow Automation
---
