---
api_key_in:
- header
api_specs:
- filename: fdx-authorization-api-openapi.yaml
  format: yaml
  label: Mastercard FDX Authorization API
  slug: authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/fdx-authorization-api-openapi.yaml
- filename: fdx-resource-api-openapi.yaml
  format: yaml
  label: Mastercard FDX Resource API
  slug: resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/openapi/fdx-resource-api-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mastercard Developer Hub For Fdx Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mastercard Developer Hub for FDX APIs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mastercard Developer Hub for FDX APIs
provider_slug: mastercard-fdx
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fdx-authorization-api-openapi.yaml
  type: http
- description: Authorization Token to access Secured API!
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/fdx-resource-api-openapi.yaml
  type: apiKey
slug: mastercard-developer-hub-for-fdx-apis-authentication
source_filename: mastercard-developer-hub-for-fdx-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fdx-authorization-api-openapi.yaml, openapi/fdx-resource-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/fdx-authorization-api-openapi.yaml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization Token to access Secured API!\n  sources:\n  - openapi/fdx-resource-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercard-fdx/refs/heads/main/authentication/mastercard-developer-hub-for-fdx-apis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Banking
- FDX
- Open Banking
---
