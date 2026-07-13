---
api_key_in: []
api_specs:
- filename: asyncapi.yml
  format: yaml
  label: Salesloft Webhooks API
  slug: salesloft-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesloft/refs/heads/main/asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Salesloft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salesloft secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Salesloft
provider_slug: salesloft
scheme_count: 3
schemes:
- name: noauthAuth
  scheme: noauth
  sources:
  - openapi/salesloft-openapi.yml
  type: http
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesloft-openapi.yml
  type: http
- name: oauth2Auth
  scheme: oauth2
  sources:
  - openapi/salesloft-openapi.yml
  type: http
slug: salesloft-authentication
source_filename: salesloft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesloft-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: noauthAuth\n  type: http\n  scheme: noauth\n  sources:\n  - openapi/salesloft-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/salesloft-openapi.yml\n- name: oauth2Auth\n  type: http\n  scheme: oauth2\n  sources:\n  - openapi/salesloft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesloft/refs/heads/main/authentication/salesloft-authentication.yml
summary_line: http · 3 schemes
tags:
- Sales
- Sales Engagement
- Cadences
- CRM
- Email
---
