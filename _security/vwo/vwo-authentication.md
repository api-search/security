---
api_key_in:
- header
api_specs:
- filename: vwo-openapi.yml
  format: yaml
  label: VWO Data API
  slug: vwo-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vwo/refs/heads/main/openapi/vwo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vwo Authentication
name_suffix: Authentication
oauth_flows: []
overview: VWO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VWO
provider_slug: vwo
scheme_count: 1
schemes:
- description: 'VWO API token sent in the `token` request header. Generate from

    VWO account settings.'
  in: header
  name: tokenAuth
  parameter: token
  sources:
  - openapi/vwo-openapi.yml
  type: apiKey
slug: vwo-authentication
source_filename: vwo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vwo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: token\n  description: |-\n    VWO API token sent in the `token` request header. Generate from\n    VWO account settings.\n  sources:\n  - openapi/vwo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vwo/refs/heads/main/authentication/vwo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Experimentation
- AB Testing
- Personalization
- Conversion Optimization
- Feature Flags
---
