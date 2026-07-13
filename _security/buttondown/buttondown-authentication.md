---
api_key_in:
- header
api_specs:
- filename: buttondown-openapi.yml
  format: yaml
  label: Buttondown API
  slug: buttondown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buttondown/refs/heads/main/openapi/buttondown-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Buttondown Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buttondown secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buttondown
provider_slug: buttondown
scheme_count: 1
schemes:
- description: API token in the form `Token <api-key>`.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/buttondown-openapi.yml
  type: apiKey
slug: buttondown-authentication
source_filename: buttondown-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/buttondown-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token in the form `Token <api-key>`.\n  sources:\n  - openapi/buttondown-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buttondown/refs/heads/main/authentication/buttondown-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Automations
- Email
- Markdown
- Newsletters
- Paid Subscriptions
- SaaS
- Subscribers
---
