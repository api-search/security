---
api_key_in:
- header
api_specs:
- filename: qualtrics-automations-api-openapi.yml
  format: yaml
  label: Qualtrics automations API
  slug: qualtrics-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-automations-api-openapi.yml
- filename: qualtrics-directories-api-openapi.yml
  format: yaml
  label: Qualtrics Directories API
  slug: qualtrics-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-directories-api-openapi.yml
- filename: qualtrics-distributions-api-openapi.yml
  format: yaml
  label: Qualtrics Distributions API
  slug: qualtrics-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-distributions-api-openapi.yml
- filename: qualtrics-eventsubscriptions-api-openapi.yml
  format: yaml
  label: Qualtrics Eventsubscriptions API
  slug: qualtrics-eventsubscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-eventsubscriptions-api-openapi.yml
- filename: qualtrics-file-api-openapi.yml
  format: yaml
  label: Qualtrics file API
  slug: qualtrics-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-file-api-openapi.yml
- filename: qualtrics-files-api-openapi.yml
  format: yaml
  label: Qualtrics files API
  slug: qualtrics-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-files-api-openapi.yml
- filename: qualtrics-survey-definitions-api-openapi.yml
  format: yaml
  label: Qualtrics Survey Definitions API
  slug: qualtrics-survey-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/openapi/qualtrics-survey-definitions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qualtrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qualtrics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qualtrics
provider_slug: qualtrics
scheme_count: 1
schemes:
- in: header
  name: QualtricsAPIKeyAuth
  parameter: X-API-TOKEN
  sources:
  - openapi/qualtrics-api-openapi-3.0.json
  - openapi/qualtrics-api-swagger-2.0.json
  - openapi/qualtrics-automations-file-service-swagger-2.0.yaml
  type: apiKey
slug: qualtrics-authentication
source_filename: qualtrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qualtrics-api-openapi-3.0.json, openapi/qualtrics-api-swagger-2.0.json, openapi/qualtrics-automations-file-service-swagger-2.0.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: QualtricsAPIKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-TOKEN\n  sources:\n  - openapi/qualtrics-api-openapi-3.0.json\n  - openapi/qualtrics-api-swagger-2.0.json\n  - openapi/qualtrics-automations-file-service-swagger-2.0.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualtrics/refs/heads/main/authentication/qualtrics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Experience Management
- Surveys
- Customer Experience
- Employee Experience
- Market Research
- XM
- REST API
---
