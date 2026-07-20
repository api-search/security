---
api_key_in:
- header
api_specs:
- filename: delphix-continuous-data-openapi.yml
  format: yaml
  label: Delphix DCT Continuous Data API
  slug: delphix-dct-continuous-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/openapi/delphix-continuous-data-openapi.yml
- filename: delphix-continuous-compliance-openapi.yml
  format: yaml
  label: Delphix DCT Continuous Compliance API
  slug: delphix-dct-continuous-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/openapi/delphix-continuous-compliance-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Delphix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delphix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Delphix
provider_slug: delphix
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/delphix-continuous-compliance-openapi.yml
  - openapi/delphix-continuous-data-openapi.yml
  token_prefix: apk
  type: apiKey
slug: delphix-authentication
source_filename: delphix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/delphix-continuous-compliance-openapi.yml, openapi/delphix-continuous-data-openapi.yml\ndocs: https://dct.delphix.com/docs/latest/api-requests-and-reporting\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  token_prefix: apk\n  note: >-\n    Data Control Tower authenticates every API request with a static API key sent in\n    the Authorization header, prefixed with \"apk\" (e.g. \"Authorization: apk 1.abc...\").\n    API keys are minted per DCT account; DCT accounts themselves can be created\n    manually or federated via LDAP/AD or SSO/SAML.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  token_prefix: apk\n  sources:\n  - openapi/delphix-continuous-compliance-openapi.yml\n  - openapi/delphix-continuous-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/authentication/delphix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Management
- Test Data Management
- Data Virtualization
- Data Masking
- Data Compliance
- Database
- DevOps
- Synthetic Data
- Data Control Tower
---
