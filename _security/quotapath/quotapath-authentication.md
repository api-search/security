---
api_key_in:
- header
api_specs:
- filename: quotapath-openapi-original.json
  format: json
  label: QuotaPath API
  slug: quotapath-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/openapi/quotapath-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Quotapath Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuotaPath secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QuotaPath
provider_slug: quotapath
scheme_count: 1
schemes:
- description: 'API Key authentication header. Prefix QuotaPath-generated api key with ''Token '' in Authorization header value. Example: ''Token abcdef12345'''
  in: header
  name: token_auth
  parameter: Authorization
  sources:
  - openapi/quotapath-openapi-original.json
  type: apiKey
slug: quotapath-authentication
source_filename: quotapath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/quotapath-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API Key authentication header. Prefix QuotaPath-generated api key with ''Token\n    '' in Authorization header value. Example: ''Token abcdef12345'''\n  sources:\n  - openapi/quotapath-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quotapath/refs/heads/main/authentication/quotapath-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Sales Commissions
- Compensation Management
- Sales Operations
- Revenue Operations
- Finance
- Payouts
- CRM Integration
- Payroll
---
