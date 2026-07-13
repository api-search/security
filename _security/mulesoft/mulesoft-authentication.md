---
api_key_in: []
api_specs:
- filename: mulesoft-anypoint-platform-openapi.yml
  format: yaml
  label: MuleSoft Anypoint Platform Management API
  slug: mulesoft-anypoint-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/openapi/mulesoft-anypoint-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mulesoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: MuleSoft secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MuleSoft
provider_slug: mulesoft
scheme_count: 1
schemes:
- description: Anypoint Platform access token obtained via the Access Management API login endpoint or a connected app OAuth 2.0 flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mulesoft-anypoint-platform-openapi.yml
  type: http
slug: mulesoft-authentication
source_filename: mulesoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mulesoft-anypoint-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Anypoint Platform access token obtained via the Access Management API login endpoint\n    or a connected app OAuth 2.0 flow.\n  sources:\n  - openapi/mulesoft-anypoint-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/authentication/mulesoft-authentication.yml
summary_line: http · 1 scheme
tags:
- API Gateway
- API Management
- Enterprise
- Integration
---
