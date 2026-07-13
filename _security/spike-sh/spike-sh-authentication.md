---
api_key_in:
- header
api_specs:
- filename: api.spike.sh
  format: yaml
  label: Spike.sh API
  slug: spike-sh
  spec_type: OpenAPI
  url: https://api.spike.sh
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spike Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spike.sh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spike.sh
provider_slug: spike-sh
scheme_count: 1
schemes:
- description: API key generated from https://app.spike.sh/api
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/spike-sh-openapi.yml
  type: apiKey
slug: spike-sh-authentication
source_filename: spike-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spike-sh-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated from https://app.spike.sh/api\n  sources:\n  - openapi/spike-sh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/authentication/spike-sh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Incident Management
- On-Call
- Alerting
- Escalation Policies
- Status Pages
- Monitoring
- DevOps
- SRE
---
