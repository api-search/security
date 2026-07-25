---
api_key_in: []
api_specs:
- filename: saasment-alerts-api-openapi.yml
  format: yaml
  label: Saasment Alerts API
  slug: saasment-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-alerts-api-openapi.yml
- filename: saasment-compliance-api-openapi.yml
  format: yaml
  label: Saasment Compliance API
  slug: saasment-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-compliance-api-openapi.yml
- filename: saasment-cost-optimization-api-openapi.yml
  format: yaml
  label: Saasment Cost Optimization API
  slug: saasment-cost-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-cost-optimization-api-openapi.yml
- filename: saasment-integrations-api-openapi.yml
  format: yaml
  label: Saasment Integrations API
  slug: saasment-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-integrations-api-openapi.yml
- filename: saasment-misconfigurations-api-openapi.yml
  format: yaml
  label: Saasment Misconfigurations API
  slug: saasment-misconfigurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-misconfigurations-api-openapi.yml
- filename: saasment-security-posture-api-openapi.yml
  format: yaml
  label: Saasment Security Posture API
  slug: saasment-security-posture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-security-posture-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Saasment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Saasment secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Saasment
provider_slug: saasment
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token from Saasment platform settings
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/saasment-openapi.yml
  type: http
slug: saasment-authentication
source_filename: saasment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/saasment-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token from Saasment platform settings\n  sources:\n  - openapi/saasment-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/authentication/saasment-authentication.yml
summary_line: http · 1 scheme
tags:
- SaaS Security
- SSPM
- Cloud Security
- Cost Optimization
- Compliance
- Misconfigurations
---
