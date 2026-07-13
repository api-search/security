---
api_key_in:
- header
api_specs:
- filename: prosci-change-management-openapi.yml
  format: yaml
  label: Prosci Change Management
  slug: prosci
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-change-management-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prosci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prosci secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Prosci
provider_slug: prosci
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the Prosci authentication endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/prosci-change-management-openapi.yml
  type: http
- description: API key provided by Prosci for application access.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/prosci-change-management-openapi.yml
  type: apiKey
slug: prosci-authentication
source_filename: prosci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prosci-change-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the Prosci authentication endpoint.\n  sources:\n  - openapi/prosci-change-management-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key provided by Prosci for application access.\n  sources:\n  - openapi/prosci-change-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/authentication/prosci-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Change Management
- Methodology
- Training
---
