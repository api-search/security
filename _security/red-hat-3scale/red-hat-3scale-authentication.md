---
api_key_in:
- query
api_specs:
- filename: red-hat-3scale-service-management-openapi.yml
  format: yaml
  label: Red Hat 3scale Service Management API
  slug: service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-service-management-openapi.yml
- filename: red-hat-3scale-account-management-openapi.yml
  format: yaml
  label: Red Hat 3scale Account Management API
  slug: account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-account-management-openapi.yml
- filename: red-hat-3scale-analytics-openapi.yml
  format: yaml
  label: Red Hat 3scale Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-analytics-openapi.yml
- filename: red-hat-3scale-billing-openapi.yml
  format: yaml
  label: Red Hat 3scale Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-billing-openapi.yml
- filename: red-hat-3scale-apicast-management-openapi.yml
  format: yaml
  label: Red Hat 3scale APIcast Management API
  slug: apicast-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-apicast-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Red Hat 3Scale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red Hat 3scale secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Red Hat 3scale
provider_slug: red-hat-3scale
scheme_count: 2
schemes:
- in: query
  name: provider_key
  parameter: access_token
  sources:
  - openapi/red-hat-3scale-account-management-openapi.yml
  - openapi/red-hat-3scale-analytics-openapi.yml
  - openapi/red-hat-3scale-billing-openapi.yml
  type: apiKey
- in: query
  name: providerKey
  parameter: provider_key
  sources:
  - openapi/red-hat-3scale-service-management-openapi.yml
  type: apiKey
slug: red-hat-3scale-authentication
source_filename: red-hat-3scale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red-hat-3scale-account-management-openapi.yml, openapi/red-hat-3scale-analytics-openapi.yml,\n  openapi/red-hat-3scale-billing-openapi.yml, openapi/red-hat-3scale-service-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: provider_key\n  type: apiKey\n  in: query\n  parameter: access_token\n  sources:\n  - openapi/red-hat-3scale-account-management-openapi.yml\n  - openapi/red-hat-3scale-analytics-openapi.yml\n  - openapi/red-hat-3scale-billing-openapi.yml\n- name: providerKey\n  type: apiKey\n  in: query\n  parameter: provider_key\n  sources:\n  - openapi/red-hat-3scale-service-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/authentication/red-hat-3scale-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Gateway
- API Management
- Developer Portal
- Enterprise
- Red Hat
---
