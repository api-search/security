---
api_key_in:
- header
api_specs:
- filename: phosphorus-api-openapi.yml
  format: yaml
  label: Phosphorus API
  slug: phosphorus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/openapi/phosphorus-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Phosphorus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phosphorus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phosphorus
provider_slug: phosphorus
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/phosphorus-api-openapi.yml
  type: apiKey
slug: phosphorus-authentication
source_filename: phosphorus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/phosphorus-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/phosphorus-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phosphorus/refs/heads/main/authentication/phosphorus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cybersecurity
- xIoT Security
- IoT Security
- OT Security
- IoMT
- Asset Discovery
- Vulnerability Management
- Firmware Management
- Certificate Management
- Credential Management
- Critical Infrastructure
- Device Management
---
