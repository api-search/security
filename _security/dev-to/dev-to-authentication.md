---
api_key_in:
- header
api_specs:
- filename: dev-to-forem-api-openapi.yml
  format: yaml
  label: Dev.to Forem API
  slug: forem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-forem-api-openapi.yml
- filename: dev-to-webhooks-asyncapi.yml
  format: yaml
  label: Dev.to Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/asyncapi/dev-to-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dev To Authentication
name_suffix: Authentication
oauth_flows: []
overview: dev-to secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dev-to
provider_slug: dev-to
scheme_count: 1
schemes:
- description: API key obtained from the DEV.to settings page. Pass in the api-key header for authenticated requests.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/dev-to-forem-api-openapi.yml
  type: apiKey
slug: dev-to-authentication
source_filename: dev-to-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dev-to-forem-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key obtained from the DEV.to settings page. Pass in the api-key header for\n    authenticated requests.\n  sources:\n  - openapi/dev-to-forem-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/authentication/dev-to-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
