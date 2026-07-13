---
api_key_in: []
api_specs:
- filename: nutshell-openapi.yml
  format: yaml
  label: Nutshell REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutshell/refs/heads/main/openapi/nutshell-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nutshell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nutshell secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nutshell
provider_slug: nutshell
scheme_count: 1
schemes:
- description: 'Authenticate with an API key generated from Nutshell account

    settings. See https://support.nutshell.com/en/articles/8429060

    for guidance on issuing API keys.'
  name: ApiKeyAuth
  scheme: basic
  sources:
  - openapi/nutshell-openapi.yml
  type: http
slug: nutshell-authentication
source_filename: nutshell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nutshell-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: basic\n  description: |-\n    Authenticate with an API key generated from Nutshell account\n    settings. See https://support.nutshell.com/en/articles/8429060\n    for guidance on issuing API keys.\n  sources:\n  - openapi/nutshell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutshell/refs/heads/main/authentication/nutshell-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Sales
- Pipeline Management
- Email Marketing
- Contact Management
- Sales Automation
---
