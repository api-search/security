---
api_key_in:
- header
api_specs:
- filename: sophos-central-siem-openapi.yml
  format: yaml
  label: Sophos Central SIEM API
  slug: sophos-central-siem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sophos/refs/heads/main/openapi/sophos-central-siem-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sophos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sophos secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sophos
provider_slug: sophos
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/sophos-central-siem-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sophos-central-siem-openapi.yml
  type: http
slug: sophos-authentication
source_filename: sophos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sophos-central-siem-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/sophos-central-siem-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sophos-central-siem-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sophos/refs/heads/main/authentication/sophos-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cybersecurity
- Endpoint Protection
- Security
- SIEM
- Threat Detection
- Incident Response
---
