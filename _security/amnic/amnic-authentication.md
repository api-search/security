---
api_key_in:
- header
api_specs:
- filename: amnic-openapi.yml
  format: yaml
  label: Amnic Cloud Cost Observability API
  slug: amnic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/openapi/amnic-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amnic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amnic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amnic
provider_slug: amnic
scheme_count: 1
schemes:
- description: API key for authenticating requests to the Amnic API. Obtain your API key from the Amnic dashboard.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/amnic-openapi.yml
  type: apiKey
slug: amnic-authentication
source_filename: amnic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amnic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating requests to the Amnic API. Obtain your API key from\n    the Amnic dashboard.\n  sources:\n  - openapi/amnic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/authentication/amnic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Cost Observability
- FinOps
- Cloud Cost Management
- Cost Optimization
- Kubernetes
- Azure
- Google Cloud
---
