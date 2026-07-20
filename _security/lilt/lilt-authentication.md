---
api_key_in:
- query
api_specs:
- filename: lilt-openapi-original.yml
  format: yaml
  label: LILT API
  slug: lilt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lilt secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lilt
provider_slug: lilt
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/lilt-openapi-original.yml
  type: http
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/lilt-openapi-original.yml
  type: apiKey
slug: lilt-authentication
source_filename: lilt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lilt-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lilt-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/lilt-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/authentication/lilt-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai
- Translation
- Localization
- Machine Translation
- Language
- Content
- Translation Memory
- Agents
---
