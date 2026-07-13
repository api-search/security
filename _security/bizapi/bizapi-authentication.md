---
api_key_in: []
api_specs:
- filename: bizapi-business-intelligence-api-openapi.yml
  format: yaml
  label: BizAPI Business Intelligence API
  slug: bizapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/openapi/bizapi-business-intelligence-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bizapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: BizAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BizAPI
provider_slug: bizapi
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using credentials provided during account activation.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bizapi-business-intelligence-api-openapi.yml
  type: http
slug: bizapi-authentication
source_filename: bizapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bizapi-business-intelligence-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using credentials provided during account activation.\n  sources:\n  - openapi/bizapi-business-intelligence-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/authentication/bizapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Intelligence
- Company Data
- CRM
- Firmographic Data
- NAICS
- SIC
---
