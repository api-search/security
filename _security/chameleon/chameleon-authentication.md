---
api_key_in:
- header
api_specs:
- filename: chameleon-openapi.yml
  format: yaml
  label: Chameleon REST API
  slug: chameleon-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Chameleon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chameleon secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chameleon
provider_slug: chameleon
scheme_count: 1
schemes:
- description: Your Chameleon account secret. See https://developers.chameleon.io/api-introduction/authentication
  in: header
  name: accountSecret
  parameter: X-Account-Secret
  sources:
  - openapi/chameleon-openapi.yml
  type: apiKey
slug: chameleon-authentication
source_filename: chameleon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chameleon-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accountSecret\n  type: apiKey\n  in: header\n  parameter: X-Account-Secret\n  description: Your Chameleon account secret. See https://developers.chameleon.io/api-introduction/authentication\n  sources:\n  - openapi/chameleon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/authentication/chameleon-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Product
- In-App Guidance
- Onboarding
- Surveys
- Analytics
---
