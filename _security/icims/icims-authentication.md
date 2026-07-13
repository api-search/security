---
api_key_in: []
api_specs:
- filename: icims-openapi.yml
  format: yaml
  label: iCIMS Workflows API
  slug: icims-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icims/refs/heads/main/openapi/icims-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Icims Authentication
name_suffix: Authentication
oauth_flows: []
overview: iCIMS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iCIMS
provider_slug: icims
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/icims-openapi.yml
  type: http
slug: icims-authentication
source_filename: icims-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/icims-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/icims-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icims/refs/heads/main/authentication/icims-authentication.yml
summary_line: http · 1 scheme
tags:
- Applicant Tracking
- HR
- Recruiting
- Talent Acquisition
---
