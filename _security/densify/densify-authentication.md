---
api_key_in: []
api_specs:
- filename: dev
  format: yaml
  label: Densify Public Cloud API
  slug: public-cloud-api
  spec_type: Postman
  url: https://www.densify.com/dev
- filename: densify-authentication-api-openapi.yml
  format: yaml
  label: Densify Authentication API
  slug: densify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-authentication-api-openapi.yml
- filename: densify-cloud-analysis-api-openapi.yml
  format: yaml
  label: Densify Cloud Analysis API
  slug: densify-cloud-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-cloud-analysis-api-openapi.yml
- filename: densify-kubernetes-api-openapi.yml
  format: yaml
  label: Densify Kubernetes API
  slug: densify-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-api-openapi.yml
- filename: densify-recommendations-api-openapi.yml
  format: yaml
  label: Densify Recommendations API
  slug: densify-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-recommendations-api-openapi.yml
- filename: densify-system-api-openapi.yml
  format: yaml
  label: Densify System API
  slug: densify-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-system-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Densify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Densify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Densify
provider_slug: densify
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/densify-openapi.yml
  type: http
slug: densify-authentication
source_filename: densify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/densify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/densify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/authentication/densify-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Cost
- Container Optimization
- FinOps
- Kubernetes
- Machine-Learning
- Recommendations
- Rightsizing
---
