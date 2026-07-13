---
api_key_in: []
api_specs:
- filename: osisoft-pi-web-api-openapi.yml
  format: yaml
  label: OSIsoft PI Web API
  slug: pi-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-web-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Osisoft Pi Authentication
name_suffix: Authentication
oauth_flows: []
overview: osisoft-pi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: osisoft-pi
provider_slug: osisoft-pi
scheme_count: 2
schemes:
- description: HTTP Basic Authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/osisoft-pi-web-api-openapi.yml
  type: http
- description: Kerberos/Windows Integrated Authentication
  name: kerberos
  scheme: negotiate
  sources:
  - openapi/osisoft-pi-web-api-openapi.yml
  type: http
slug: osisoft-pi-authentication
source_filename: osisoft-pi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/osisoft-pi-web-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication\n  sources:\n  - openapi/osisoft-pi-web-api-openapi.yml\n- name: kerberos\n  type: http\n  scheme: negotiate\n  description: Kerberos/Windows Integrated Authentication\n  sources:\n  - openapi/osisoft-pi-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/authentication/osisoft-pi-authentication.yml
summary_line: http · 2 schemes
tags: []
---
