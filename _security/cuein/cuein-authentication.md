---
api_key_in:
- header
api_specs:
- filename: cuein-insights-openapi.json
  format: json
  label: Cuein Insights API
  slug: cuein-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/openapi/cuein-insights-openapi.json
- filename: cuein-answers-openapi.json
  format: json
  label: Cuein Answers API
  slug: cuein-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/openapi/cuein-answers-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cuein Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cuein secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cuein
provider_slug: cuein
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/cuein-answers-openapi.json
  - openapi/cuein-insights-openapi.json
  type: apiKey
slug: cuein-authentication
source_filename: cuein-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cuein-answers-openapi.json, openapi/cuein-insights-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/cuein-answers-openapi.json\n  - openapi/cuein-insights-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/authentication/cuein-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Experience
- Customer Support
- Conversation Intelligence
- Generative AI
- Insights
- Knowledge Base
- Contact Center
---
