---
api_key_in:
- header
api_specs:
- filename: activecampaign-v3.json
  format: json
  label: ActiveCampaign API v3
  slug: activecampaign-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/openapi/activecampaign-v3.json
- filename: activecampaign-sms.json
  format: json
  label: ActiveCampaign SMS Broadcast API
  slug: activecampaign-sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/openapi/activecampaign-sms.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Activecampaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActiveCampaign secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ActiveCampaign
provider_slug: activecampaign
scheme_count: 1
schemes:
- description: Your ActiveCampaign API token
  in: header
  name: ApiToken
  parameter: Api-Token
  sources:
  - openapi/activecampaign-sms.json
  - openapi/activecampaign-v3.json
  type: apiKey
slug: activecampaign-authentication
source_filename: activecampaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activecampaign-sms.json, openapi/activecampaign-v3.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: Api-Token\n  description: Your ActiveCampaign API token\n  sources:\n  - openapi/activecampaign-sms.json\n  - openapi/activecampaign-v3.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/authentication/activecampaign-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
---
