---
api_key_in:
- header
api_specs:
- filename: trakstar-hire-api-openapi.yml
  format: yaml
  label: Trakstar Hire API
  slug: trakstar-hire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-hire-api-openapi.yml
- filename: trakstar-learn-api-openapi.yml
  format: yaml
  label: Trakstar Learn API
  slug: trakstar-learn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-learn-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trakstar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trakstar secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trakstar
provider_slug: trakstar
scheme_count: 2
schemes:
- description: API key generated from the Trakstar Hire Super Admin settings page. Pass as "ApiKey {your_api_key}".
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/trakstar-hire-api-openapi.yml
  type: apiKey
- description: API key provisioned by Trakstar Learn support team. Contact learn@trakstar.com to request access.
  in: header
  name: apiKey
  parameter: x-mindflash-apikey
  sources:
  - openapi/trakstar-learn-api-openapi.yml
  type: apiKey
slug: trakstar-authentication
source_filename: trakstar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trakstar-hire-api-openapi.yml, openapi/trakstar-learn-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key generated from the Trakstar Hire Super Admin settings page. Pass as \"ApiKey\n    {your_api_key}\".\n  sources:\n  - openapi/trakstar-hire-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-mindflash-apikey\n  description: API key provisioned by Trakstar Learn support team. Contact learn@trakstar.com\n    to request access.\n  sources:\n  - openapi/trakstar-learn-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/authentication/trakstar-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- HR
- Human Resources
- Performance Management
- Talent Management
- Applicant Tracking
- Learning Management
- 360 Feedback
- Goal Management
- Employee Development
- Performance Appraisal
---
