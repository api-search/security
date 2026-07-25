---
api_key_in: []
api_specs:
- filename: nubela-company-api-openapi.yml
  format: yaml
  label: Nubela Company API
  slug: nubela-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/openapi/nubela-company-api-openapi.yml
- filename: nubela-competitor-api-openapi.yml
  format: yaml
  label: Nubela Competitor API
  slug: nubela-competitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/openapi/nubela-competitor-api-openapi.yml
- filename: nubela-customer-api-openapi.yml
  format: yaml
  label: Nubela Customer API
  slug: nubela-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/openapi/nubela-customer-api-openapi.yml
- filename: nubela-employee-api-openapi.yml
  format: yaml
  label: Nubela Employee API
  slug: nubela-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/openapi/nubela-employee-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nubela Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nubela secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nubela
provider_slug: nubela
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nubela-openapi.yml
  type: http
slug: nubela-authentication
source_filename: nubela-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nubela-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nubela-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nubela/refs/heads/main/authentication/nubela-authentication.yml
summary_line: http · 1 scheme
tags:
- Companies
- Data
- People
- Scraping
---
