---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: FusionAuth API
  slug: fusionauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/FusionAuth/fusionauth-openapi/main/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fusionauth Authentication
name_suffix: Authentication
oauth_flows: []
overview: FusionAuth secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FusionAuth
provider_slug: fusionauth
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/fusionauth-openapi.yaml
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fusionauth-openapi.yaml
  type: http
slug: fusionauth-authentication
source_filename: fusionauth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fusionauth-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/fusionauth-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fusionauth-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusionauth/refs/heads/main/authentication/fusionauth-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Authentication
- Authorization
- Identity
- CIAM
- OAuth
- OpenID Connect
- Single Sign-On
- Multi-Factor Authentication
---
