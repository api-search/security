---
api_key_in: []
api_specs:
- filename: unisys-stealth-ecoapi-openapi.yaml
  format: yaml
  label: Unisys Stealth EcoAPI
  slug: unisys-stealth-ecoapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unisys/refs/heads/main/openapi/unisys-stealth-ecoapi-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unisys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unisys secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unisys
provider_slug: unisys
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Stealth server credentials (username and password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/unisys-stealth-ecoapi-openapi.yaml
  type: http
slug: unisys-authentication
source_filename: unisys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unisys-stealth-ecoapi-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Stealth server credentials (username and password).\n  sources:\n  - openapi/unisys-stealth-ecoapi-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisys/refs/heads/main/authentication/unisys-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 1000
- Security
- Zero Trust
- Network Security
- IT Services
- Cybersecurity
- Enterprise Technology
---
