---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Workleap API
  slug: workleap-api
  spec_type: OpenAPI
  url: https://docs.api.workleap.com/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Workleap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workleap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workleap
provider_slug: workleap
scheme_count: 1
schemes:
- description: API key for authenticating requests to the Workleap API
  in: header
  name: SubscriptionKey
  parameter: workleap-subscription-key
  sources:
  - openapi/workleap-workleap-api-openapi.yml
  type: apiKey
slug: workleap-authentication
source_filename: workleap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workleap-workleap-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: workleap-subscription-key\n  description: API key for authenticating requests to the Workleap API\n  sources:\n  - openapi/workleap-workleap-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/authentication/workleap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Employee Experience
- HR
- Engagement
- Pulse Surveys
- Performance Management
- Officevibe
- User Provisioning
- HRIS
- Recognition
- Onboarding
---
