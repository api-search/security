---
api_key_in: []
api_specs:
- filename: hint-health-hint-health-api-openapi.yml
  format: yaml
  label: Hint Health API
  slug: hint-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/openapi/hint-health-hint-health-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hint Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hint Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hint Health
provider_slug: hint-health
scheme_count: 1
schemes:
- description: Practice access token or Partner API key (Bearer authentication)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/hint-health-hint-health-api-openapi.yml
  type: http
slug: hint-health-authentication
source_filename: hint-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hint-health-hint-health-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Practice access token or Partner API key (Bearer authentication)\n  sources:\n  - openapi/hint-health-hint-health-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/authentication/hint-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Direct Primary Care
- DPC
- Healthcare
- Membership Management
- Patient Enrollment
- Medical Billing
- EMR
- Health Plans
---
