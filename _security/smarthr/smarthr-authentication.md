---
api_key_in: []
api_specs:
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Crews API
  slug: smarthr-crews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Departments API
  slug: smarthr-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Employment Types API
  slug: smarthr-employment-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Custom Field Templates API
  slug: smarthr-custom-field-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Business Establishments API
  slug: smarthr-business-establishments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Webhooks API
  slug: smarthr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smarthr Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmartHR secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SmartHR
provider_slug: smarthr
scheme_count: 1
schemes:
- description: 'Per-tenant access token issued from the SmartHR admin console (OAuth2 access tokens are used for registered apps), passed as `Authorization: Bearer ACCESS_TOKEN`. HTTP Basic auth with the access token as the username (`curl -u ACCESS_TOKEN`) is also accepted.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smarthr-openapi.yml
  - https://developer.smarthr.jp/api/about_api
  type: http
slug: smarthr-authentication
source_filename: smarthr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/smarthr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Per-tenant access token issued from the SmartHR admin console (OAuth2 access\n    tokens are used for registered apps), passed as `Authorization: Bearer\n    ACCESS_TOKEN`. HTTP Basic auth with the access token as the username\n    (`curl -u ACCESS_TOKEN`) is also accepted.\n  sources:\n  - openapi/smarthr-openapi.yml\n  - https://developer.smarthr.jp/api/about_api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/authentication/smarthr-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- Human Resources
- HRIS
- Labor Management
- Payroll
- Japan
- Employees
- Personnel
- Onboarding
- SaaS
---
