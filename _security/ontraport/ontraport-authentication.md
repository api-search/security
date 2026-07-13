---
api_key_in:
- header
api_specs:
- filename: ontraport-openapi.yml
  format: yaml
  label: Ontraport REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ontraport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ontraport secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ontraport
provider_slug: ontraport
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/ontraport-openapi.yml
  type: apiKey
- in: header
  name: AppIdAuth
  parameter: Api-Appid
  sources:
  - openapi/ontraport-openapi.yml
  type: apiKey
slug: ontraport-authentication
source_filename: ontraport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ontraport-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  sources:\n  - openapi/ontraport-openapi.yml\n- name: AppIdAuth\n  type: apiKey\n  in: header\n  parameter: Api-Appid\n  sources:\n  - openapi/ontraport-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/authentication/ontraport-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- CRM
- Marketing Automation
- Email Marketing
- Ecommerce
- Landing Pages
- Membership Sites
---
