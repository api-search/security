---
api_key_in:
- header
api_specs:
- filename: ordway-rest-api-openapi.yml
  format: yaml
  label: Ordway REST API
  slug: ordway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordway/refs/heads/main/openapi/ordway-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ordway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ordway secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ordway
provider_slug: ordway
scheme_count: 4
schemes:
- description: Ordway API key
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/ordway-rest-api-openapi.yml
  type: apiKey
- description: Ordway user authentication token
  in: header
  name: UserTokenAuth
  parameter: X-User-Token
  sources:
  - openapi/ordway-rest-api-openapi.yml
  type: apiKey
- description: Ordway user email address
  in: header
  name: UserEmailAuth
  parameter: X-User-Email
  sources:
  - openapi/ordway-rest-api-openapi.yml
  type: apiKey
- description: Ordway company identifier
  in: header
  name: CompanyAuth
  parameter: X-User-Company
  sources:
  - openapi/ordway-rest-api-openapi.yml
  type: apiKey
slug: ordway-authentication
source_filename: ordway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ordway-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Ordway API key\n  sources:\n  - openapi/ordway-rest-api-openapi.yml\n- name: UserTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Token\n  description: Ordway user authentication token\n  sources:\n  - openapi/ordway-rest-api-openapi.yml\n- name: UserEmailAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Email\n  description: Ordway user email address\n  sources:\n  - openapi/ordway-rest-api-openapi.yml\n- name: CompanyAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Company\n  description: Ordway company identifier\n  sources:\n  - openapi/ordway-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordway/refs/heads/main/authentication/ordway-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Billing
- Revenue Automation
- Subscriptions
- Invoicing
- Payments
- Revenue Recognition
- SaaS Metrics
- Usage-Based Billing
- Financial Reporting
- Accounts Receivable
---
