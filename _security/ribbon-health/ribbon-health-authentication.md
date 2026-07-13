---
api_key_in: []
api_specs:
- filename: ribbon-health-h1-api-openapi.yml
  format: yaml
  label: H1 API (Ribbon Health)
  slug: h1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-h1-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ribbon Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ribbon Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ribbon Health
provider_slug: ribbon-health
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ribbon-health-h1-api-openapi.yml
  type: http
slug: ribbon-health-authentication
source_filename: ribbon-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ribbon-health-h1-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ribbon-health-h1-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/authentication/ribbon-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Provider Directory
- Insurance
- Clinical Data
- Care Navigation
- Eligibility
- Price Transparency
- Provider Search
- Health Plans
- Digital Health
---
