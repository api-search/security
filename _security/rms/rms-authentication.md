---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rms-openapi.yml
  format: yaml
  label: Risk Modeler API
  slug: risk-modeler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rms/openapi/rms-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Moody's RMS Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moody's RMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moody's RMS
provider_slug: rms
scheme_count: 1
schemes:
- description: An API key is a token that enables a client application to make requests to tenant applications running on Intelligent Risk Platform.
  in: header
  name: RMS_Auth
  parameter: Authorization
  sources:
  - openapi/rms-openapi.yml
  type: apiKey
slug: rms-authentication
source_filename: rms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/rms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: RMS_Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: An API key is a token that enables a client application to make requests to tenant\n    applications running on Intelligent Risk Platform.\n  sources:\n  - openapi/rms-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/rms/authentication/rms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Insurance
- Risk Management
- Modeling
- Analytics
- Technology
- Company
---
