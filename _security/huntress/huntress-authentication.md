---
api_key_in: []
api_specs:
- filename: huntress-rest-openapi.json
  format: json
  label: Huntress REST API
  slug: huntress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-rest-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Huntress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Huntress secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Huntress
provider_slug: huntress
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/huntress-rest-openapi.json
  type: http
slug: huntress-authentication
source_filename: huntress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/huntress-rest-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/huntress-rest-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/authentication/huntress-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Endpoint Security
- SOC
- SIEM
- Identity Threat Detection
- MSP
- Webhooks
---
