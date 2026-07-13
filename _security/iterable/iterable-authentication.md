---
api_key_in:
- header
api_specs:
- filename: iterable-rest-api-openapi.yml
  format: yaml
  label: Iterable REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-rest-api-openapi.yml
- filename: iterable-export-api-openapi.yml
  format: yaml
  label: Iterable Export API
  slug: export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-export-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Iterable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iterable secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Iterable
provider_slug: iterable
scheme_count: 1
schemes:
- description: Iterable API key passed in the Api-Key header. API keys can be created and managed in the Iterable project settings.
  in: header
  name: apiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/iterable-export-api-openapi.yml
  - openapi/iterable-rest-api-openapi.yml
  type: apiKey
slug: iterable-authentication
source_filename: iterable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iterable-export-api-openapi.yml, openapi/iterable-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Iterable API key passed in the Api-Key header. API keys can be created and managed\n    in the Iterable project settings.\n  sources:\n  - openapi/iterable-export-api-openapi.yml\n  - openapi/iterable-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/authentication/iterable-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
---
