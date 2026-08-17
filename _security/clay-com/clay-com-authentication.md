---
api_key_in:
- header
api_specs:
- filename: clay-com-public-api-openapi.json
  format: json
  label: Clay Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-public-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clay Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clay secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clay
provider_slug: clay-com
scheme_count: 1
schemes:
- description: Personal API key tied to your Clay user. Create one under Settings → Account in the Clay app.
  in: header
  name: ClayApiKey
  parameter: clay-api-key
  sources:
  - openapi/clay-com-public-api-openapi.json
  type: apiKey
slug: clay-com-authentication
source_filename: clay-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/clay-com-public-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ClayApiKey\n  type: apiKey\n  in: header\n  parameter: clay-api-key\n  description: Personal API key tied to your Clay user. Create one under Settings → Account\n    in the Clay app.\n  sources:\n  - openapi/clay-com-public-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/authentication/clay-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Prospecting
- GTM
- Sales
- Enrichment
- Automation
- AI
- Webhooks
---
