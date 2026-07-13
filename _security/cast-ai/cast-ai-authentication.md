---
api_key_in:
- header
api_specs:
- filename: cast-ai-kubernetes-cost-optimization-openapi.yml
  format: yaml
  label: CAST AI Kubernetes Cost Optimization API
  slug: kubernetes-cost-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-kubernetes-cost-optimization-openapi.yml
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
