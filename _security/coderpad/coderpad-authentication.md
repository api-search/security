---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coderpad-account-api-openapi.yml
  format: yaml
  label: CoderPad Account API
  slug: coderpad-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-account-api-openapi.yml
- filename: coderpad-campaigns-api-openapi.yml
  format: yaml
  label: CoderPad Campaigns API
  slug: coderpad-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-campaigns-api-openapi.yml
- filename: coderpad-me-api-openapi.yml
  format: yaml
  label: CoderPad Me API
  slug: coderpad-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-me-api-openapi.yml
- filename: coderpad-organization-api-openapi.yml
  format: yaml
  label: CoderPad Organization API
  slug: coderpad-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-organization-api-openapi.yml
- filename: coderpad-pad-environments-api-openapi.yml
  format: yaml
  label: CoderPad Pad environments API
  slug: coderpad-pad-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-pad-environments-api-openapi.yml
- filename: coderpad-pads-api-openapi.yml
  format: yaml
  label: CoderPad Pads API
  slug: coderpad-pads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-pads-api-openapi.yml
- filename: coderpad-question-variants-api-openapi.yml
  format: yaml
  label: CoderPad Question variants API
  slug: coderpad-question-variants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-question-variants-api-openapi.yml
- filename: coderpad-questions-api-openapi.yml
  format: yaml
  label: CoderPad Questions API
  slug: coderpad-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-questions-api-openapi.yml
- filename: coderpad-temporaryfile-api-openapi.yml
  format: yaml
  label: CoderPad Temporary File API
  slug: coderpad-temporaryfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-temporaryfile-api-openapi.yml
- filename: coderpad-tests-api-openapi.yml
  format: yaml
  label: CoderPad Tests API
  slug: coderpad-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-tests-api-openapi.yml
- filename: coderpad-webhook-api-openapi.yml
  format: yaml
  label: CoderPad Webhook API
  slug: coderpad-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-webhook-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Coderpad Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoderPad secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CoderPad
provider_slug: coderpad
scheme_count: 2
schemes:
- description: 'Your API key, from [your settings page](https://app.coderpad.io/settings). The `Authorization: Token token="YOUR_API_KEY"` format is also accepted.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/coderpad-interview-api-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: API-Key
  sources:
  - openapi/coderpad-screen-api-openapi.yml
  type: apiKey
slug: coderpad-authentication
source_filename: coderpad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/coderpad-interview-api-openapi.yml, openapi/coderpad-screen-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Your API key, from [your settings page](https://app.coderpad.io/settings). The\n    `Authorization: Token token=\"YOUR_API_KEY\"` format is also accepted.'\n  sources:\n  - openapi/coderpad-interview-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: API-Key\n  sources:\n  - openapi/coderpad-screen-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/coderpad/authentication/coderpad-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Hiring
- TechnicalAssessment
- InterviewPlatform
---
