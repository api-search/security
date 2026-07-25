---
api_key_in:
- header
api_specs:
- filename: harness-cloud-cost-anomalies-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Anomalies API
  slug: harness-cloud-cost-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-anomalies-api-openapi.yml
- filename: harness-cloud-cost-budgets-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Budgets API
  slug: harness-cloud-cost-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-budgets-api-openapi.yml
- filename: harness-cloud-cost-connectors-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Connectors API
  slug: harness-cloud-cost-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-connectors-api-openapi.yml
- filename: harness-cloud-cost-cost-categories-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Cost Categories API
  slug: harness-cloud-cost-cost-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-cost-categories-api-openapi.yml
- filename: harness-cloud-cost-perspectives-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Perspectives API
  slug: harness-cloud-cost-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-perspectives-api-openapi.yml
- filename: harness-cloud-cost-recommendations-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Recommendations API
  slug: harness-cloud-cost-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-recommendations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Harness Cloud Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harness Cloud Cost Management secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harness Cloud Cost Management
provider_slug: harness-cloud-cost
scheme_count: 1
schemes:
- description: Harness Personal Access Token or Service Account API key.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/harness-cloud-cost-openapi.yml
  type: apiKey
slug: harness-cloud-cost-authentication
source_filename: harness-cloud-cost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harness-cloud-cost-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Harness Personal Access Token or Service Account API key.\n  sources:\n  - openapi/harness-cloud-cost-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/authentication/harness-cloud-cost-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Anomaly Detection
- Budgets
- Cloud Cost Management
- FinOps
- Kubernetes
- Recommendations
---
