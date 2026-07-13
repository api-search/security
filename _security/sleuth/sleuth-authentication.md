---
api_key_in:
- header
api_specs:
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Deployments Registration API
  slug: deployments-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Manual Change API
  slug: manual-change-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Metric and Incident Impact API
  slug: metric-impact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sleuth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sleuth secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sleuth
provider_slug: sleuth
scheme_count: 1
schemes:
- description: 'Sleuth Access Token / organization API key supplied as "Authorization: apikey <APIKEY>". A Bearer token form ("Authorization: Bearer <ACCESS_TOKEN>") is also accepted for deploy registration. Scoped Access Tokens are managed under Organization Settings > Access Tokens.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/sleuth-openapi.yml
  type: apiKey
slug: sleuth-authentication
source_filename: sleuth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sleuth-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Sleuth Access Token / organization API key supplied as \"Authorization: apikey\n    <APIKEY>\". A Bearer token form (\"Authorization: Bearer <ACCESS_TOKEN>\") is also accepted\n    for deploy registration. Scoped Access Tokens are managed under Organization Settings >\n    Access Tokens.'\n  sources:\n  - openapi/sleuth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/authentication/sleuth-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DORA
- DevOps
- Deployment Tracking
- Engineering Metrics
- Continuous Delivery
---
