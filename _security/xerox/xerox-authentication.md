---
api_key_in:
- header
api_specs:
- filename: xerox-public-print-openapi.yml
  format: yaml
  label: Xerox Public Print API
  slug: xerox-public-print-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xerox/refs/heads/main/openapi/xerox-public-print-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Xerox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xerox secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xerox
provider_slug: xerox
scheme_count: 3
schemes:
- description: Xerox authentication credentials
  in: header
  name: xrxauth
  parameter: xrxauth
  sources:
  - openapi/xerox-public-print-openapi.yml
  type: apiKey
- description: User email address for user-context requests
  in: header
  name: userEmail
  parameter: user-email
  sources:
  - openapi/xerox-public-print-openapi.yml
  type: apiKey
- description: Application identifier
  in: header
  name: appId
  parameter: appid
  sources:
  - openapi/xerox-public-print-openapi.yml
  type: apiKey
slug: xerox-authentication
source_filename: xerox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xerox-public-print-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: xrxauth\n  type: apiKey\n  in: header\n  parameter: xrxauth\n  description: Xerox authentication credentials\n  sources:\n  - openapi/xerox-public-print-openapi.yml\n- name: userEmail\n  type: apiKey\n  in: header\n  parameter: user-email\n  description: User email address for user-context requests\n  sources:\n  - openapi/xerox-public-print-openapi.yml\n- name: appId\n  type: apiKey\n  in: header\n  parameter: appid\n  description: Application identifier\n  sources:\n  - openapi/xerox-public-print-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xerox/refs/heads/main/authentication/xerox-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Document Management
- Enterprise
- Fortune 500
- Managed Print Services
- Print Services
- Printing
---
