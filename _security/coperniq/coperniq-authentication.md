---
api_key_in:
- header
api_specs:
- filename: coperniq-openapi.yml
  format: yaml
  label: Coperniq API
  slug: coperniq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coperniq/refs/heads/main/openapi/coperniq-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coperniq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coperniq secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coperniq
provider_slug: coperniq
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/coperniq-api-key-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/coperniq-openapi.yml
  type: apiKey
slug: coperniq-authentication
source_filename: coperniq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coperniq-api-key-openapi.yml, openapi/coperniq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/coperniq-api-key-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/coperniq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coperniq/refs/heads/main/authentication/coperniq-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Climate
- Solar
- Construction
- Field Service Management
- Project Management
- Contractors
- CRM
- Energy
---
