---
api_key_in:
- header
api_specs:
- filename: usergems-api-openapi.yml
  format: yaml
  label: UserGems API
  slug: usergems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Usergems Authentication
name_suffix: Authentication
oauth_flows: []
overview: UserGems secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UserGems
provider_slug: usergems
scheme_count: 1
schemes:
- description: 'Customer-issued API key. Request a key from support@usergems.com. The

    key must be included on every request in the X-Api-Key header.'
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/usergems-api-openapi.yml
  type: apiKey
slug: usergems-authentication
source_filename: usergems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/usergems-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: |-\n    Customer-issued API key. Request a key from support@usergems.com. The\n    key must be included on every request in the X-Api-Key header.\n  sources:\n  - openapi/usergems-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/authentication/usergems-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sales Intelligence
- Outbound
- ABM
- Champion Tracking
- Job Changes
- Buying Signals
- AI Scoring
- Sales Engagement
- CRM
- Revenue Operations
- GTM
---
