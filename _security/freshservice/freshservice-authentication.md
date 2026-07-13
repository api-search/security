---
api_key_in: []
api_specs:
- filename: freshservice-openapi.yml
  format: yaml
  label: Freshservice API v2
  slug: itsm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshservice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshservice secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshservice
provider_slug: freshservice
scheme_count: 1
schemes:
- description: HTTP Basic with API key as username and "X" as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/freshservice-openapi.yml
  type: http
slug: freshservice-authentication
source_filename: freshservice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshservice-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with API key as username and \"X\" as password.\n  sources:\n  - openapi/freshservice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/authentication/freshservice-authentication.yml
summary_line: http · 1 scheme
tags:
- ITSM
- IT Service Management
- Help Desk
- Ticketing
- Asset Management
- Change Management
- Freshworks
---
