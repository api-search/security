---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Consumer Complaint Database API
  slug: consumer-complaint-database-api
  spec_type: OpenAPI
  url: https://cfpb.github.io/ccdb5-api/documentation/
- filename: cfpb-hmda-data-browser-api-openapi.yml
  format: yaml
  label: HMDA Data Browser API
  slug: hmda-data-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/main/openapi/cfpb-hmda-data-browser-api-openapi.yml
- filename: cfpb-hmda-filing-api-openapi.yml
  format: yaml
  label: HMDA Platform Filing API
  slug: hmda-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/main/openapi/cfpb-hmda-filing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cfpb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consumer Financial Protection Bureau (CFPB) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Consumer Financial Protection Bureau (CFPB)
provider_slug: cfpb
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cfpb-hmda-filing-api-openapi.yml
  type: http
slug: cfpb-authentication
source_filename: cfpb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cfpb-hmda-filing-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cfpb-hmda-filing-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/authentication/cfpb-authentication.yml
summary_line: http · 1 scheme
tags:
- Consumer Finance
- Government
- Complaints
- Mortgage
- HMDA
- Financial Data
- Regulatory
- Open Data
---
