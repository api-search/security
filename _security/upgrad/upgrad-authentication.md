---
api_key_in:
- header
api_specs:
- filename: upgrad-partner-openapi.yml
  format: yaml
  label: upGrad Partner Service API
  slug: upgrad-partner-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-partner-openapi.yml
- filename: upgrad-learner-analytics-openapi.yml
  format: yaml
  label: upGrad Learner Experience Analytics API
  slug: upgrad-learner-experience-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-learner-analytics-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Upgrad Authentication
name_suffix: Authentication
oauth_flows: []
overview: upGrad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: upGrad
provider_slug: upgrad
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: Authorization
  scheme: bearer
  sources:
  - openapi/upgrad-learner-analytics-openapi.yml
  type: http
- in: header
  name: AUTH-TOKEN
  parameter: AUTH-TOKEN
  sources:
  - openapi/upgrad-partner-openapi.yml
  type: apiKey
slug: upgrad-authentication
source_filename: upgrad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/upgrad-learner-analytics-openapi.yml, openapi/upgrad-partner-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/upgrad-learner-analytics-openapi.yml\n- name: AUTH-TOKEN\n  type: apiKey\n  in: header\n  parameter: AUTH-TOKEN\n  sources:\n  - openapi/upgrad-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/authentication/upgrad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- EdTech
- Online Learning
- Higher Education
- Certification
- Learning Analytics
- Partner Management
- India
---
