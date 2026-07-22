---
api_key_in: []
api_specs:
- filename: verato-person-openapi.yml
  format: yaml
  label: Verato Person API
  slug: verato-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/openapi/verato-person-openapi.yml
- filename: verato-organization-openapi.yml
  format: yaml
  label: Verato Organization API
  slug: verato-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/openapi/verato-organization-openapi.yml
- filename: verato-provider-openapi.yml
  format: yaml
  label: Verato Provider API
  slug: verato-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/openapi/verato-provider-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Verato Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verato secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Verato
provider_slug: verato
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/verato-organization-openapi.yml
  - openapi/verato-person-openapi.yml
  - openapi/verato-provider-openapi.yml
  type: http
slug: verato-authentication
source_filename: verato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/verato-organization-openapi.yml, openapi/verato-person-openapi.yml, openapi/verato-provider-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/verato-organization-openapi.yml\n  - openapi/verato-person-openapi.yml\n  - openapi/verato-provider-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verato/refs/heads/main/authentication/verato-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Healthcare
- Identity
- Identity Resolution
- Master Data Management
- Patient Matching
- Provider Data Management
- Data Quality
- EMPI
---
