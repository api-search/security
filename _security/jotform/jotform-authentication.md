---
api_key_in:
- header
- query
api_specs:
- filename: jotform-folder-api-openapi.yml
  format: yaml
  label: Jotform Folder API
  slug: jotform-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-folder-api-openapi.yml
- filename: jotform-form-api-openapi.yml
  format: yaml
  label: Jotform Form API
  slug: jotform-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-form-api-openapi.yml
- filename: jotform-label-api-openapi.yml
  format: yaml
  label: Jotform Label API
  slug: jotform-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-label-api-openapi.yml
- filename: jotform-report-api-openapi.yml
  format: yaml
  label: Jotform Report API
  slug: jotform-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-report-api-openapi.yml
- filename: jotform-submission-api-openapi.yml
  format: yaml
  label: Jotform Submission API
  slug: jotform-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-submission-api-openapi.yml
- filename: jotform-system-api-openapi.yml
  format: yaml
  label: Jotform System API
  slug: jotform-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-system-api-openapi.yml
- filename: jotform-user-api-openapi.yml
  format: yaml
  label: Jotform User API
  slug: jotform-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-user-api-openapi.yml
- filename: jotform-webhook-api-openapi.yml
  format: yaml
  label: Jotform Webhook API
  slug: jotform-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/openapi/jotform-webhook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jotform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jotform secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jotform
provider_slug: jotform
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: APIKEY
  sources:
  - openapi/jotform-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/jotform-openapi.yml
  type: apiKey
slug: jotform-authentication
source_filename: jotform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jotform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: APIKEY\n  sources:\n  - openapi/jotform-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/jotform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jotform/refs/heads/main/authentication/jotform-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Forms
- Surveys
- No-Code
- Data Collection
- Workflow
- HIPAA
- EU
---
