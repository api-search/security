---
api_key_in:
- header
api_specs:
- filename: toys-r-us-commerce-openapi.yml
  format: yaml
  label: Toys R Us Commerce API
  slug: logicbroker-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toys-r-us/refs/heads/main/openapi/toys-r-us-commerce-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Toys R Us Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toys R Us secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Toys R Us
provider_slug: toys-r-us
scheme_count: 1
schemes:
- description: API subscription key obtained from the Toys R Us LogicBroker supplier portal. Set up your key at https://stageportal.logicbroker.com/profile/api-authentication/
  in: header
  name: apiKeyAuth
  parameter: subscription-key
  sources:
  - openapi/toys-r-us-commerce-openapi.yml
  type: apiKey
slug: toys-r-us-authentication
source_filename: toys-r-us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toys-r-us-commerce-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: subscription-key\n  description: API subscription key obtained from the Toys R Us LogicBroker supplier portal.\n    Set up your key at https://stageportal.logicbroker.com/profile/api-authentication/\n  sources:\n  - openapi/toys-r-us-commerce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toys-r-us/refs/heads/main/authentication/toys-r-us-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- Dropship
- E-Commerce
- Retail
- Supply Chain
- Fortune 500
---
