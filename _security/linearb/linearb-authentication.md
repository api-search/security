---
api_key_in:
- header
api_specs:
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Deployments API
  slug: linearb-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Incidents API
  slug: linearb-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Measurements API
  slug: linearb-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Teams API
  slug: linearb-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Services API
  slug: linearb-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Webhooks API
  slug: linearb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Linearb Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinearB secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LinearB
provider_slug: linearb
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/linearb-openapi.yml
  type: apiKey
slug: linearb-authentication
source_filename: linearb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linearb-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/linearb-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/authentication/linearb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Engineering Analytics
- SEI
- Developer Productivity
- DORA Metrics
- DevOps
---
