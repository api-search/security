---
api_key_in:
- header
api_specs:
- filename: microsoft-azure-communication-services-openapi.yml
  format: yaml
  label: Azure Communication Services REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-communication-services/refs/heads/main/openapi/microsoft-azure-communication-services-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Communication Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: microsoft-azure-communication-services secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: microsoft-azure-communication-services
provider_slug: microsoft-azure-communication-services
scheme_count: 1
schemes:
- description: HMAC-SHA256 signed Authorization header
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-communication-services-openapi.yml
  type: apiKey
slug: microsoft-azure-communication-services-authentication
source_filename: microsoft-azure-communication-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-communication-services-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA256 signed Authorization header\n  sources:\n  - openapi/microsoft-azure-communication-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-communication-services/refs/heads/main/authentication/microsoft-azure-communication-services-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
