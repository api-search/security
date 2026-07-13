---
api_key_in: []
api_specs:
- filename: direct-mail-api
  format: yaml
  label: Stannp Direct Mail API
  slug: direct-mail-api
  spec_type: OpenAPI
  url: https://www.stannp.com/us/direct-mail-api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stannp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stannp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stannp
provider_slug: stannp
scheme_count: 1
schemes:
- description: Use your API key as the username and leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/stannp-direct-mail-api-openapi.yml
  type: http
slug: stannp-authentication
source_filename: stannp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stannp-direct-mail-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your API key as the username and leave the password blank.\n  sources:\n  - openapi/stannp-direct-mail-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/authentication/stannp-authentication.yml
summary_line: http · 1 scheme
tags:
- Direct Mail
- Postcards
- Letters
- Print
- Physical Mail
- Marketing Automation
- Campaigns
---
