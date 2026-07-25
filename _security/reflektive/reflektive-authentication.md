---
api_key_in:
- header
api_specs:
- filename: reflektive-real-time-feedback-v1-api-openapi.yml
  format: yaml
  label: Reflektive Real-time Feedback (v1) API
  slug: reflektive-real-time-feedback-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reflektive/refs/heads/main/openapi/reflektive-real-time-feedback-v1-api-openapi.yml
- filename: reflektive-real-time-feedback-v2-api-openapi.yml
  format: yaml
  label: Reflektive Real-time Feedback (v2) API
  slug: reflektive-real-time-feedback-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reflektive/refs/heads/main/openapi/reflektive-real-time-feedback-v2-api-openapi.yml
- filename: reflektive-reports-api-openapi.yml
  format: yaml
  label: Reflektive Reports API
  slug: reflektive-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reflektive/refs/heads/main/openapi/reflektive-reports-api-openapi.yml
- filename: reflektive-tasks-api-openapi.yml
  format: yaml
  label: Reflektive Tasks API
  slug: reflektive-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reflektive/refs/heads/main/openapi/reflektive-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reflektive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reflektive secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reflektive
provider_slug: reflektive
scheme_count: 1
schemes:
- description: 'Token-based authentication. Pass the header as: `Authorization: Token token=<your_api_key>`. Contact support@reflektive.com to obtain an API key.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/reflektive-reflektive-api-openapi.yml
  type: apiKey
slug: reflektive-authentication
source_filename: reflektive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reflektive-reflektive-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Pass the header as: `Authorization: Token token=<your_api_key>`.\n    Contact support@reflektive.com to obtain an API key.'\n  sources:\n  - openapi/reflektive-reflektive-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflektive/refs/heads/main/authentication/reflektive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Performance Management
- HR
- Employee Feedback
- Goal Tracking
- Engagement Surveys
- Reviews
- People Analytics
- REST API
---
