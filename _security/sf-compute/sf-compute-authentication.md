---
api_key_in: []
api_specs:
- filename: sf-compute-account-api-openapi.yml
  format: yaml
  label: San Francisco Compute Company Account API
  slug: sf-compute-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-account-api-openapi.yml
- filename: sf-compute-images-api-openapi.yml
  format: yaml
  label: San Francisco Compute Company Images API
  slug: sf-compute-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-images-api-openapi.yml
- filename: sf-compute-money-api-openapi.yml
  format: yaml
  label: San Francisco Compute Company Money API
  slug: sf-compute-money-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-money-api-openapi.yml
- filename: sf-compute-nodes-api-openapi.yml
  format: yaml
  label: San Francisco Compute Company Nodes API
  slug: sf-compute-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-nodes-api-openapi.yml
- filename: sf-compute-orders-api-openapi.yml
  format: yaml
  label: San Francisco Compute Company Orders API
  slug: sf-compute-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-orders-api-openapi.yml
- filename: sf-compute-vms-api-openapi.yml
  format: yaml
  label: San Francisco Compute Company VMs API
  slug: sf-compute-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-vms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sf Compute Authentication
name_suffix: Authentication
oauth_flows: []
overview: San Francisco Compute Company secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: San Francisco Compute Company
provider_slug: sf-compute
scheme_count: 1
schemes:
- bearerFormat: Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sf-compute-openapi.yml
  type: http
slug: sf-compute-authentication
source_filename: sf-compute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sf-compute-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  sources:\n  - openapi/sf-compute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/authentication/sf-compute-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Cloud
- Clusters
- Compute
- GPU
- Machine Learning
- Marketplace
- Training
---
