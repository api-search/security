---
api_key_in:
- query
api_specs:
- filename: leadsquared-openapi.yml
  format: yaml
  label: LeadSquared REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/openapi/leadsquared-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Leadsquared Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadSquared secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeadSquared
provider_slug: leadsquared
scheme_count: 2
schemes:
- in: query
  name: AccessKeyAuth
  parameter: accessKey
  sources:
  - openapi/leadsquared-openapi.yml
  type: apiKey
- in: query
  name: SecretKeyAuth
  parameter: secretKey
  sources:
  - openapi/leadsquared-openapi.yml
  type: apiKey
slug: leadsquared-authentication
source_filename: leadsquared-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leadsquared-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: AccessKeyAuth\n  type: apiKey\n  in: query\n  parameter: accessKey\n  sources:\n  - openapi/leadsquared-openapi.yml\n- name: SecretKeyAuth\n  type: apiKey\n  in: query\n  parameter: secretKey\n  sources:\n  - openapi/leadsquared-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/authentication/leadsquared-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Marketing Automation
- CRM
- Sales Automation
- Lead Management
- Customer Engagement
- Field Force Automation
---
