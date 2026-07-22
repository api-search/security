---
api_key_in:
- header
api_specs:
- filename: rocketlane-openapi-original.json
  format: json
  label: Rocketlane API
  slug: rocketlane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketlane/refs/heads/main/openapi/rocketlane-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rocketlane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rocketlane secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rocketlane
provider_slug: rocketlane
scheme_count: 1
schemes:
- description: Requests authenticate with a per-workspace API key passed in the 'api-key' request header. Keys are generated from Rocketlane workspace settings.
  in: header
  name: apiKeyAuth
  parameter_name: api-key
  type: apiKey
slug: rocketlane-authentication
source_filename: rocketlane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.rocketlane.com/docs/overview + https://developer.rocketlane.com/docs/api-explorer\ndocs: https://developer.rocketlane.com/docs/overview\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: api-key\n  description: Requests authenticate with a per-workspace API key passed in the\n    'api-key' request header. Keys are generated from Rocketlane workspace settings.\nnotes: Rocketlane uses a static API-key header ('api-key') for all API access; no\n  OAuth 2.0 / OpenID Connect flow is documented, so scopes/ is intentionally not\n  produced (key auth has no scope surface).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketlane/refs/heads/main/authentication/rocketlane-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Professional Services Automation
- Project Management
- Customer Onboarding
- Resource Management
- Time Tracking
- PSA
- SaaS
---
