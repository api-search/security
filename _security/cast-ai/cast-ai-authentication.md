---
api_key_in:
- header
api_specs:
- filename: cast-ai-ai-enabler-api-openapi.yml
  format: yaml
  label: CAST AI AI Enabler API
  slug: cast-ai-ai-enabler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-ai-enabler-api-openapi.yml
- filename: cast-ai-allocation-groups-api-openapi.yml
  format: yaml
  label: CAST AI Allocation Groups API
  slug: cast-ai-allocation-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-allocation-groups-api-openapi.yml
- filename: cast-ai-autoscaler-api-openapi.yml
  format: yaml
  label: CAST AI Autoscaler API
  slug: cast-ai-autoscaler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-autoscaler-api-openapi.yml
- filename: cast-ai-cluster-actions-api-openapi.yml
  format: yaml
  label: CAST AI Cluster Actions API
  slug: cast-ai-cluster-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-cluster-actions-api-openapi.yml
- filename: cast-ai-cost-reports-api-openapi.yml
  format: yaml
  label: CAST AI Cost Reports API
  slug: cast-ai-cost-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-cost-reports-api-openapi.yml
- filename: cast-ai-external-clusters-api-openapi.yml
  format: yaml
  label: CAST AI External Clusters API
  slug: cast-ai-external-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-external-clusters-api-openapi.yml
- filename: cast-ai-hibernation-schedules-api-openapi.yml
  format: yaml
  label: CAST AI Hibernation Schedules API
  slug: cast-ai-hibernation-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-hibernation-schedules-api-openapi.yml
- filename: cast-ai-insights-api-openapi.yml
  format: yaml
  label: CAST AI Insights API
  slug: cast-ai-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-insights-api-openapi.yml
- filename: cast-ai-inventory-api-openapi.yml
  format: yaml
  label: CAST AI Inventory API
  slug: cast-ai-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-inventory-api-openapi.yml
- filename: cast-ai-node-configuration-api-openapi.yml
  format: yaml
  label: CAST AI Node Configuration API
  slug: cast-ai-node-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-node-configuration-api-openapi.yml
- filename: cast-ai-node-templates-api-openapi.yml
  format: yaml
  label: CAST AI Node Templates API
  slug: cast-ai-node-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-node-templates-api-openapi.yml
- filename: cast-ai-operations-api-openapi.yml
  format: yaml
  label: CAST AI Operations API
  slug: cast-ai-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-operations-api-openapi.yml
- filename: cast-ai-policies-api-openapi.yml
  format: yaml
  label: CAST AI Policies API
  slug: cast-ai-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-policies-api-openapi.yml
- filename: cast-ai-pricing-api-openapi.yml
  format: yaml
  label: CAST AI Pricing API
  slug: cast-ai-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-pricing-api-openapi.yml
- filename: cast-ai-scheduled-rebalancing-api-openapi.yml
  format: yaml
  label: CAST AI Scheduled Rebalancing API
  slug: cast-ai-scheduled-rebalancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-scheduled-rebalancing-api-openapi.yml
- filename: cast-ai-settings-api-openapi.yml
  format: yaml
  label: CAST AI Settings API
  slug: cast-ai-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-settings-api-openapi.yml
- filename: cast-ai-workload-optimization-api-openapi.yml
  format: yaml
  label: CAST AI Workload Optimization API
  slug: cast-ai-workload-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-workload-optimization-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cast Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: CAST AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CAST AI
provider_slug: cast-ai
scheme_count: 1
schemes:
- description: API key for authentication. Create access keys from the CAST AI console under API > API access keys.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/cast-ai-kubernetes-cost-optimization-openapi.yml
  type: apiKey
slug: cast-ai-authentication
source_filename: cast-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cast-ai-kubernetes-cost-optimization-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication. Create access keys from the CAST AI console under\n    API > API access keys.\n  sources:\n  - openapi/cast-ai-kubernetes-cost-optimization-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/authentication/cast-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
---
