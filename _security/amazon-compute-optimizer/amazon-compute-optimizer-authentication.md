---
api_key_in:
- header
api_specs:
- filename: amazon-compute-optimizer-openapi.yml
  format: yaml
  label: Amazon Compute Optimizer API
  slug: amazon-compute-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/openapi/amazon-compute-optimizer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Compute Optimizer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Compute Optimizer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-compute-optimizer-openapi.yml
  type: apiKey
slug: amazon-compute-optimizer-authentication
source_filename: amazon-compute-optimizer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-compute-optimizer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-compute-optimizer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/authentication/amazon-compute-optimizer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
---
