---
api_key_in:
- header
api_specs:
- filename: gravity-forms-openapi.yml
  format: yaml
  label: Gravity Forms REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravity-forms/refs/heads/main/openapi/gravity-forms-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gravity Forms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gravity Forms secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gravity Forms
provider_slug: gravity-forms
scheme_count: 2
schemes:
- description: Basic auth using a Gravity Forms REST API key/secret.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/gravity-forms-openapi.yml
  type: http
- description: OAuth 1.0a signed requests using API key/secret.
  in: header
  name: oauth1
  parameter: Authorization
  sources:
  - openapi/gravity-forms-openapi.yml
  type: apiKey
slug: gravity-forms-authentication
source_filename: gravity-forms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gravity-forms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic auth using a Gravity Forms REST API key/secret.\n  sources:\n  - openapi/gravity-forms-openapi.yml\n- name: oauth1\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: OAuth 1.0a signed requests using API key/secret.\n  sources:\n  - openapi/gravity-forms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravity-forms/refs/heads/main/authentication/gravity-forms-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- WordPress
- Forms
- Form Builder
- Surveys
- Workflow
- Plugins
---
