---
api_key_in:
- header
api_specs:
- filename: cloudzero-allocation-telemetry-api-openapi.yml
  format: yaml
  label: CloudZero Allocation Telemetry API
  slug: cloudzero-allocation-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-allocation-telemetry-api-openapi.yml
- filename: cloudzero-anycost-api-openapi.yml
  format: yaml
  label: CloudZero AnyCost API
  slug: cloudzero-anycost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-anycost-api-openapi.yml
- filename: cloudzero-billing-api-openapi.yml
  format: yaml
  label: CloudZero Billing API
  slug: cloudzero-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-billing-api-openapi.yml
- filename: cloudzero-budgets-api-openapi.yml
  format: yaml
  label: CloudZero Budgets API
  slug: cloudzero-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-budgets-api-openapi.yml
- filename: cloudzero-insights-api-openapi.yml
  format: yaml
  label: CloudZero Insights API
  slug: cloudzero-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-insights-api-openapi.yml
- filename: cloudzero-unit-metric-telemetry-api-openapi.yml
  format: yaml
  label: CloudZero Unit Metric Telemetry API
  slug: cloudzero-unit-metric-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/openapi/cloudzero-unit-metric-telemetry-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudzero Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudZero secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudZero
provider_slug: cloudzero
scheme_count: 1
schemes:
- description: API key for authentication. Include your API key directly in the Authorization header.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/cloudzero-api-openapi.yml
  type: apiKey
slug: cloudzero-authentication
source_filename: cloudzero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudzero-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key for authentication. Include your API key directly in the Authorization\n    header.\n  sources:\n  - openapi/cloudzero-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/authentication/cloudzero-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
---
