---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: blumira-health-api-openapi.yml
  format: yaml
  label: Blumira Health API
  slug: blumira-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-health-api-openapi.yml
- filename: blumira-msp-api-openapi.yml
  format: yaml
  label: Blumira Msp API
  slug: blumira-msp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-msp-api-openapi.yml
- filename: blumira-org-api-openapi.yml
  format: yaml
  label: Blumira Org API
  slug: blumira-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-org-api-openapi.yml
- filename: blumira-resolutions-api-openapi.yml
  format: yaml
  label: Blumira Resolutions API
  slug: blumira-resolutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-resolutions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Blumira Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blumira secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blumira
provider_slug: blumira
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: pax8ApiTokenV1
  sources:
  - openapi/blumira-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blumira-openapi.yml
  type: http
slug: blumira-authentication
source_filename: blumira-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: derived\nsource: openapi/blumira-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: pax8ApiTokenV1\n  sources:\n  - openapi/blumira-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/blumira-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/authentication/blumira-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Security
- Software-as-a-Service
- Cloud
- IT
---
