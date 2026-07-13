---
api_key_in:
- header
api_specs:
- filename: amd-developer-cloud-api-openapi.yml
  format: yaml
  label: AMD Developer Cloud API
  slug: amd-developer-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/amd-developer-cloud-api-openapi.yml
- filename: amd-rocm-management-api-openapi.yml
  format: yaml
  label: AMD ROCm API
  slug: amd-rocm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/amd-rocm-management-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Advanced Micro Devices Authentication
name_suffix: Authentication
oauth_flows: []
overview: Advanced Micro Devices secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/amd-developer-cloud-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/amd-rocm-management-api-openapi.yml
  type: http
slug: advanced-micro-devices-authentication
source_filename: advanced-micro-devices-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amd-developer-cloud-api-openapi.yml, openapi/amd-rocm-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/amd-developer-cloud-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/amd-rocm-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/authentication/advanced-micro-devices-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
- Fortune 500
---
