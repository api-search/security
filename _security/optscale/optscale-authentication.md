---
api_key_in: []
api_specs:
- filename: optscale-authentication-api-openapi.yml
  format: yaml
  label: OptScale Authentication API
  slug: optscale-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-authentication-api-openapi.yml
- filename: optscale-cloud-accounts-api-openapi.yml
  format: yaml
  label: OptScale Cloud Accounts API
  slug: optscale-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-cloud-accounts-api-openapi.yml
- filename: optscale-employees-api-openapi.yml
  format: yaml
  label: OptScale Employees API
  slug: optscale-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-employees-api-openapi.yml
- filename: optscale-expenses-api-openapi.yml
  format: yaml
  label: OptScale Expenses API
  slug: optscale-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-expenses-api-openapi.yml
- filename: optscale-optimizations-api-openapi.yml
  format: yaml
  label: OptScale Optimizations API
  slug: optscale-optimizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-optimizations-api-openapi.yml
- filename: optscale-organizations-api-openapi.yml
  format: yaml
  label: OptScale Organizations API
  slug: optscale-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-organizations-api-openapi.yml
- filename: optscale-pools-api-openapi.yml
  format: yaml
  label: OptScale Pools API
  slug: optscale-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-pools-api-openapi.yml
- filename: optscale-recommendations-api-openapi.yml
  format: yaml
  label: OptScale Recommendations API
  slug: optscale-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-recommendations-api-openapi.yml
- filename: optscale-resources-api-openapi.yml
  format: yaml
  label: OptScale Resources API
  slug: optscale-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-resources-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Optscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: OptScale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OptScale
provider_slug: optscale
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/optscale-openapi.yml
  type: http
slug: optscale-authentication
source_filename: optscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/optscale-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/optscale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/authentication/optscale-authentication.yml
summary_line: http · 1 scheme
tags:
- FinOps
- Cost Optimization
- Cloud
- Kubernetes
- Open-Source
---
