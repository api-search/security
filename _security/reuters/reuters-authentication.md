---
api_key_in:
- query
api_specs:
- filename: reuters-connect-api-openapi.yml
  format: yaml
  label: Reuters Connect API
  slug: reuters-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/openapi/reuters-connect-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reuters Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reuters secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reuters
provider_slug: reuters
scheme_count: 1
schemes:
- description: Authorization token obtained from the /login endpoint. Must be included as a query parameter in all content API requests.
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/reuters-connect-api-openapi.yml
  type: apiKey
slug: reuters-authentication
source_filename: reuters-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reuters-connect-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: Authorization token obtained from the /login endpoint. Must be included as a\n    query parameter in all content API requests.\n  sources:\n  - openapi/reuters-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/authentication/reuters-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business
- Finance
- Journalism
- Media
- News
- Wire Service
---
