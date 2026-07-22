---
api_key_in:
- header
api_specs:
- filename: orange-health-partner-openapi.yml
  format: yaml
  label: Orange Health Partner API
  slug: orange-health-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-health/refs/heads/main/openapi/orange-health-partner-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Orange Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orange Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orange Health
provider_slug: orange-health
scheme_count: 1
schemes:
- description: 'Partner API key sent in the api_key header. Public sandbox keys: partner-alwaysPartner, partner-alwaysOH, partner-decidedAtOrderLevel. Production keys via integrations@orangehealth.in.'
  in: header
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/orange-health-partner-openapi.yml
  type: apiKey
slug: orange-health-authentication
source_filename: orange-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/orange-health-partner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: 'Partner API key sent in the api_key header. Public sandbox keys: partner-alwaysPartner,\n    partner-alwaysOH, partner-decidedAtOrderLevel. Production keys via integrations@orangehealth.in.'\n  sources:\n  - openapi/orange-health-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-health/refs/heads/main/authentication/orange-health-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mobile
- Healthcare
- Diagnostics
- Lab Testing
- Home Collection
- Webhooks
- India
---
