---
api_key_in: []
api_specs:
- filename: fathom-analytics-api-openapi.yml
  format: yaml
  label: Fathom Analytics REST API
  slug: fathom-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fathom/refs/heads/main/openapi/fathom-analytics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fathom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fathom Analytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fathom Analytics
provider_slug: fathom
scheme_count: 1
schemes:
- description: API key generated in account settings at https://app.usefathom.com/api
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fathom-analytics-api-openapi.yml
  type: http
slug: fathom-authentication
source_filename: fathom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fathom-analytics-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key generated in account settings at https://app.usefathom.com/api\n  sources:\n  - openapi/fathom-analytics-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fathom/refs/heads/main/authentication/fathom-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Privacy
- GDPR
- Website Analytics
- Cookieless
- Page Views
- Events
- Reporting
---
