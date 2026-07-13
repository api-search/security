---
api_key_in:
- header
api_specs:
- filename: active-campaign-openapi.yml
  format: yaml
  label: ActiveCampaign API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Active Campaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActiveCampaign secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ActiveCampaign
provider_slug: active-campaign
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Api-Token
  sources:
  - openapi/active-campaign-openapi.yml
  type: apiKey
slug: active-campaign-authentication
source_filename: active-campaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/active-campaign-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Token\n  sources:\n  - openapi/active-campaign-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/authentication/active-campaign-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketing Automation
- Email Marketing
- CRM
- Customer Experience Automation
- Sales Engagement
---
