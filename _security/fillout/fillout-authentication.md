---
api_key_in: []
api_specs:
- filename: fillout-openapi.yml
  format: yaml
  label: Fillout REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fillout/refs/heads/main/openapi/fillout-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fillout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fillout secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fillout
provider_slug: fillout
scheme_count: 1
schemes:
- description: 'Enter your [Fillout API key](https://build.fillout.com/home/settings/developer). Format: Bearer <api_key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fillout-openapi.yml
  type: http
slug: fillout-authentication
source_filename: fillout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fillout-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Enter your [Fillout API key](https://build.fillout.com/home/settings/developer).\n    Format: Bearer <api_key>'\n  sources:\n  - openapi/fillout-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fillout/refs/heads/main/authentication/fillout-authentication.yml
summary_line: http · 1 scheme
tags:
- Forms
- Surveys
- No-Code
- Airtable
- Notion
- Salesforce
- HubSpot
- Workflow
---
