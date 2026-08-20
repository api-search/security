---
api_key_in:
- header
api_specs:
- filename: advanced-micro-devices-configuration-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Configuration API
  slug: advanced-micro-devices-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-configuration-api-openapi.yml
- filename: advanced-micro-devices-credits-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Credits API
  slug: advanced-micro-devices-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-credits-api-openapi.yml
- filename: advanced-micro-devices-devices-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Devices API
  slug: advanced-micro-devices-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-devices-api-openapi.yml
- filename: advanced-micro-devices-health-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Health API
  slug: advanced-micro-devices-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-health-api-openapi.yml
- filename: advanced-micro-devices-instances-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Instances API
  slug: advanced-micro-devices-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-instances-api-openapi.yml
- filename: advanced-micro-devices-models-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Models API
  slug: advanced-micro-devices-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-models-api-openapi.yml
- filename: advanced-micro-devices-monitoring-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Monitoring API
  slug: advanced-micro-devices-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-monitoring-api-openapi.yml
- filename: advanced-micro-devices-performance-api-openapi.yml
  format: yaml
  label: Advanced Micro Devices Performance API
  slug: advanced-micro-devices-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/openapi/advanced-micro-devices-performance-api-openapi.yml
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
- Artificial Intelligence
- Cloud Computing
- GPU
- HPC
- Machine-Learning
- Semiconductors
- Fortune 500
---
