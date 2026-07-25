---
api_key_in: []
api_specs:
- filename: vendasta-account-api-openapi.yml
  format: yaml
  label: Vendasta account API
  slug: vendasta-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-account-api-openapi.yml
- filename: vendasta-activity-api-openapi.yml
  format: yaml
  label: Vendasta activity API
  slug: vendasta-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-activity-api-openapi.yml
- filename: vendasta-change-spend-api-openapi.yml
  format: yaml
  label: Vendasta change_spend API
  slug: vendasta-change-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-change-spend-api-openapi.yml
- filename: vendasta-customer-api-openapi.yml
  format: yaml
  label: Vendasta customer API
  slug: vendasta-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-customer-api-openapi.yml
- filename: vendasta-executive-report-api-openapi.yml
  format: yaml
  label: Vendasta executive_report API
  slug: vendasta-executive-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-executive-report-api-openapi.yml
- filename: vendasta-marketplace-app-api-openapi.yml
  format: yaml
  label: Vendasta marketplace_app API
  slug: vendasta-marketplace-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-marketplace-app-api-openapi.yml
- filename: vendasta-oauth-api-openapi.yml
  format: yaml
  label: Vendasta oauth API
  slug: vendasta-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-oauth-api-openapi.yml
- filename: vendasta-user-api-openapi.yml
  format: yaml
  label: Vendasta user API
  slug: vendasta-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vendasta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vendasta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vendasta
provider_slug: vendasta
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vendasta-marketplace-openapi-original.yml
  type: http
slug: vendasta-authentication
source_filename: vendasta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vendasta-marketplace-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/vendasta-marketplace-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/authentication/vendasta-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SaaS
- Marketplace
- SMB
- White Label
- Reseller
- Marketing
- CRM
- Digital Agency
- Platform
---
