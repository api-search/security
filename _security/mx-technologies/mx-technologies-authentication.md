---
api_key_in: []
api_specs:
- filename: mx_platform_api.yml
  format: yaml
  label: MX Platform API
  slug: mx-platform-api
  spec_type: OpenAPI
  url: https://github.com/mxenabled/openapi/blob/master/openapi/mx_platform_api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mx Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: MX Technologies secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MX Technologies
provider_slug: mx-technologies
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mx-technologies-platform-openapi.yml
  - openapi/mx-technologies-platform-v20250224-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/mx-technologies-platform-openapi.yml
  - openapi/mx-technologies-platform-v20250224-openapi.yml
  type: http
slug: mx-technologies-authentication
source_filename: mx-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mx-technologies-platform-openapi.yml, openapi/mx-technologies-platform-v20250224-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mx-technologies-platform-openapi.yml\n  - openapi/mx-technologies-platform-v20250224-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/mx-technologies-platform-openapi.yml\n  - openapi/mx-technologies-platform-v20250224-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mx-technologies/refs/heads/main/authentication/mx-technologies-authentication.yml
summary_line: http · 2 schemes
tags:
- Financial Data
- Account Aggregation
- Open Banking
- Data Connectivity
- Fintech
- Transaction Categorization
- Data Enhancement
- FDX
- Account Verification
- Personal Finance
---
