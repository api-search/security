---
api_key_in: []
api_specs:
- filename: drip-openapi.yml
  format: yaml
  label: Drip REST API
  slug: drip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drip secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Drip
provider_slug: drip
scheme_count: 2
schemes:
- description: API token used as username with empty password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/drip-openapi.yml
  type: http
- bearerFormat: OAuth2 access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drip-openapi.yml
  type: http
slug: drip-authentication
source_filename: drip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drip-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API token used as username with empty password\n  sources:\n  - openapi/drip-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2 access token\n  sources:\n  - openapi/drip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/authentication/drip-authentication.yml
summary_line: http · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- Customer Engagement
- Campaigns
- Workflows
---
