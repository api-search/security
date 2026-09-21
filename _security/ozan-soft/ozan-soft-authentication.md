---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: ozan-soft-openapi.yml
  format: yaml
  label: GenderAPI.io
  slug: genderapiio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozan-soft/refs/heads/main/openapi/ozan-soft-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Ozan Soft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ozan Soft secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ozan Soft
provider_slug: ozan-soft
scheme_count: 2
schemes:
- description: Recommended server-side API-key transport.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ozan-soft-openapi.yml
  type: http
- description: Supported by documented GET endpoints; keep requests server-side.
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/ozan-soft-openapi.yml
  type: apiKey
slug: ozan-soft-authentication
source_filename: ozan-soft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: derived\nsource: openapi/ozan-soft-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Recommended server-side API-key transport.\n  sources:\n  - openapi/ozan-soft-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Supported by documented GET endpoints; keep requests server-side.\n  sources:\n  - openapi/ozan-soft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozan-soft/refs/heads/main/authentication/ozan-soft-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data Enrichment
- Gender Detection
- Name Analysis
- Demographics
- Identity
- Marketing Data
- Developer API
- Phone Validation
---
