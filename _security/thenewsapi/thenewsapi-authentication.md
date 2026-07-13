---
api_key_in:
- query
api_specs:
- filename: openapi.json
  format: json
  label: TheNewsAPI
  slug: thenewsapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenewsapi/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Thenewsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheNewsAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TheNewsAPI
provider_slug: thenewsapi
scheme_count: 1
schemes:
- description: API token obtained after free registration at https://www.thenewsapi.com/register
  in: query
  name: ApiToken
  parameter: api_token
  sources:
  - openapi/openapi.json
  type: apiKey
slug: thenewsapi-authentication
source_filename: thenewsapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: API token obtained after free registration at https://www.thenewsapi.com/register\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thenewsapi/refs/heads/main/authentication/thenewsapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- news
- articles
- headlines
- media
- aggregation
- real-time
---
