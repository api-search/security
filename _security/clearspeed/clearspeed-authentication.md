---
api_key_in:
- header
api_specs:
- filename: clearspeed-integration-api-openapi.yml
  format: yaml
  label: Clearspeed Integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/openapi/clearspeed-integration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Clearspeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clearspeed secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clearspeed
provider_slug: clearspeed
scheme_count: 1
schemes:
- in: header
  name: authorization
  parameter: Authorization
  sources:
  - openapi/clearspeed-integration-api-openapi.yml
  type: apiKey
slug: clearspeed-authentication
source_filename: clearspeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/clearspeed-integration-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/clearspeed-integration-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/authentication/clearspeed-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Risk Assessment
- Fraud Detection
- Voice Analytics
- Artificial Intelligence
- Insurance
- Identity Verification
- Screening
- Security
---
