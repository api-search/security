---
api_key_in:
- query
api_specs:
- filename: federal-motor-carrier-safety-administration-openapi.yml
  format: yaml
  label: Federal Motor Carrier Safety Administration QCMobile API
  slug: federal-motor-carrier-safety-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-motor-carrier-safety-administration/refs/heads/main/openapi/federal-motor-carrier-safety-administration-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Federal Motor Carrier Safety Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Motor Carrier Safety Administration secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Federal Motor Carrier Safety Administration
provider_slug: federal-motor-carrier-safety-administration
scheme_count: 1
schemes:
- in: query
  name: WebKey
  parameter: webKey
  sources:
  - openapi/federal-motor-carrier-safety-administration-openapi.yml
  type: apiKey
slug: federal-motor-carrier-safety-administration-authentication
source_filename: federal-motor-carrier-safety-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/federal-motor-carrier-safety-administration-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: WebKey\n  type: apiKey\n  in: query\n  parameter: webKey\n  sources:\n  - openapi/federal-motor-carrier-safety-administration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-motor-carrier-safety-administration/refs/heads/main/authentication/federal-motor-carrier-safety-administration-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Safety
- Transportation
---
