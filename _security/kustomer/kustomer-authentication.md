---
api_key_in: []
api_specs:
- filename: kustomer-openapi.yml
  format: yaml
  label: Kustomer REST API
  slug: kustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kustomer/refs/heads/main/openapi/kustomer-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kustomer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kustomer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kustomer
provider_slug: kustomer
scheme_count: 1
schemes:
- description: 'Provide an API key issued from Settings > Security > API Keys in the Kustomer console. Header format: `Authorization: Bearer {API_KEY}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kustomer-openapi.yml
  type: http
slug: kustomer-authentication
source_filename: kustomer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kustomer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Provide an API key issued from Settings > Security > API Keys in the Kustomer\n    console. Header format: `Authorization: Bearer {API_KEY}`.'\n  sources:\n  - openapi/kustomer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kustomer/refs/heads/main/authentication/kustomer-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Service
- CRM
- Helpdesk
- Messaging
- AI
---
