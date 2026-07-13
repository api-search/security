---
api_key_in:
- header
api_specs:
- filename: contrast-security-openapi.yml
  format: yaml
  label: Contrast TeamServer REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contrast-security/refs/heads/main/openapi/contrast-security-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Contrast Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contrast Security secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Contrast Security
provider_slug: contrast-security
scheme_count: 2
schemes:
- in: header
  name: Contrast-API-Key
  parameter: API-Key
  sources:
  - openapi/contrast-security-openapi.yml
  type: apiKey
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/contrast-security-openapi.yml
  type: apiKey
slug: contrast-security-authentication
source_filename: contrast-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contrast-security-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Contrast-API-Key\n  type: apiKey\n  in: header\n  parameter: API-Key\n  sources:\n  - openapi/contrast-security-openapi.yml\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/contrast-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contrast-security/refs/heads/main/authentication/contrast-security-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Application Security
- AppSec
- IAST
- RASP
- SCA
- DevSecOps
- Runtime Protection
---
