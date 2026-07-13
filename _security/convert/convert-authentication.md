---
api_key_in:
- cookie
- header
api_specs:
- filename: convert-openapi.yml
  format: yaml
  label: Convert Experiences REST API v2
  slug: convert-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convert/refs/heads/main/openapi/convert-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Convert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convert secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convert
provider_slug: convert
scheme_count: 3
schemes:
- description: See **[API Key Authentication](#tag/API-KEY-Authentication)** for more information.
  in: header
  name: requestSigning
  parameter: Authorization
  sources:
  - openapi/convert-openapi.yml
  type: apiKey
- description: See **[API Key Authentication](#tag/API-KEY-Authentication)** for more information.
  name: secretKey
  scheme: bearer
  sources:
  - openapi/convert-openapi.yml
  type: http
- description: Cookie authentication is used against Convert's own IdentityProvider  or third party identity providers and is described more in the "[Cookie Authentication](#tag/Cookie-Authentication)" section
  in: cookie
  name: cookieAuthentication
  parameter: sid
  sources:
  - openapi/convert-openapi.yml
  type: apiKey
slug: convert-authentication
source_filename: convert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/convert-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: requestSigning\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: See **[API Key Authentication](#tag/API-KEY-Authentication)** for more information.\n  sources:\n  - openapi/convert-openapi.yml\n- name: secretKey\n  type: http\n  scheme: bearer\n  description: See **[API Key Authentication](#tag/API-KEY-Authentication)** for more information.\n  sources:\n  - openapi/convert-openapi.yml\n- name: cookieAuthentication\n  type: apiKey\n  in: cookie\n  parameter: sid\n  description: Cookie authentication is used against Convert's own IdentityProvider  or third\n    party identity providers and is described more in the \"[Cookie Authentication](#tag/Cookie-Authentication)\"\n    section\n  sources:\n  - openapi/convert-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convert/refs/heads/main/authentication/convert-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Experimentation
- AB Testing
- Conversion Optimization
- Personalization
- Analytics
---
