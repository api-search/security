---
api_key_in:
- header
api_specs:
- filename: client-api-external
  format: yaml
  label: AlayaCare Client API
  slug: alayacare-client-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/AlayaCare/client-api-external
- filename: alayacare-scheduler-openapi.yml
  format: yaml
  label: AlayaCare Scheduler API
  slug: alayacare-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/openapi/alayacare-scheduler-openapi.yml
- filename: alayacare-forms-openapi.yml
  format: yaml
  label: AlayaCare Forms API
  slug: alayacare-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/openapi/alayacare-forms-openapi.yml
- filename: alayacare-accounting-openapi.yml
  format: yaml
  label: AlayaCare Accounting API
  slug: alayacare-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/openapi/alayacare-accounting-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alayacare Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlayaCare secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AlayaCare
provider_slug: api-evangelist-alayacare
scheme_count: 2
schemes:
- description: Basic HTTP auth over https
  name: basic_auth
  scheme: basic
  sources:
  - openapi/alayacare-accounting-openapi.yml
  - openapi/alayacare-careplan-openapi.yml
  - openapi/alayacare-client-openapi.yml
  - openapi/alayacare-clinical-openapi.yml
  - openapi/alayacare-employee-openapi.yml
  - openapi/alayacare-employee-skills-openapi.yml
  - openapi/alayacare-employee-unavailability-openapi.yml
  - openapi/alayacare-forms-openapi.yml
  - openapi/alayacare-medication-openapi.yml
  - openapi/alayacare-scheduler-openapi.yml
  - openapi/alayacare-services-openapi.yml
  - openapi/alayacare-tasks-openapi.yml
  type: http
- in: header
  name: CognitoAuthorizer
  parameter: Authorization
  sources:
  - openapi/alayacare-market-openapi.yml
  type: apiKey
slug: alayacare-authentication
source_filename: alayacare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alayacare-accounting-openapi.yml, openapi/alayacare-careplan-openapi.yml, openapi/alayacare-client-openapi.yml,\n  openapi/alayacare-clinical-openapi.yml, openapi/alayacare-employee-openapi.yml, openapi/alayacare-employee-skills-openapi.yml,\n  openapi/alayacare-employee-unavailability-openapi.yml, openapi/alayacare-forms-openapi.yml,\n  openapi/alayacare-market-openapi.yml, openapi/alayacare-medication-openapi.yml, openapi/alayacare-scheduler-openapi.yml,\n  openapi/alayacare-services-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: Basic HTTP auth over https\n  sources:\n  - openapi/alayacare-accounting-openapi.yml\n  - openapi/alayacare-careplan-openapi.yml\n  - openapi/alayacare-client-openapi.yml\n  - openapi/alayacare-clinical-openapi.yml\n  - openapi/alayacare-employee-openapi.yml\n  - openapi/alayacare-employee-skills-openapi.yml\n\
  \  - openapi/alayacare-employee-unavailability-openapi.yml\n  - openapi/alayacare-forms-openapi.yml\n  - openapi/alayacare-medication-openapi.yml\n  - openapi/alayacare-scheduler-openapi.yml\n  - openapi/alayacare-services-openapi.yml\n  - openapi/alayacare-tasks-openapi.yml\n- name: CognitoAuthorizer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/alayacare-market-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/authentication/alayacare-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Home Care
- Community Care
- Healthcare
- Scheduling
- Clinical
- Billing
- Client Management
- Care Management
- Aged Care
- Workforce Management
---
