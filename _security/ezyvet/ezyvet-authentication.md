---
api_key_in: []
api_specs:
- filename: ezyvet-animals-api-openapi.yml
  format: yaml
  label: ezyVet Animals API
  slug: ezyvet-animals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-animals-api-openapi.yml
- filename: ezyvet-appointments-api-openapi.yml
  format: yaml
  label: ezyVet Appointments API
  slug: ezyvet-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-appointments-api-openapi.yml
- filename: ezyvet-authentication-api-openapi.yml
  format: yaml
  label: ezyVet Authentication API
  slug: ezyvet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-authentication-api-openapi.yml
- filename: ezyvet-consultations-api-openapi.yml
  format: yaml
  label: ezyVet Consultations API
  slug: ezyvet-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-consultations-api-openapi.yml
- filename: ezyvet-contacts-api-openapi.yml
  format: yaml
  label: ezyVet Contacts API
  slug: ezyvet-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-contacts-api-openapi.yml
- filename: ezyvet-diagnostics-api-openapi.yml
  format: yaml
  label: ezyVet Diagnostics API
  slug: ezyvet-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-diagnostics-api-openapi.yml
- filename: ezyvet-invoices-api-openapi.yml
  format: yaml
  label: ezyVet Invoices API
  slug: ezyvet-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-invoices-api-openapi.yml
- filename: ezyvet-prescriptions-api-openapi.yml
  format: yaml
  label: ezyVet Prescriptions API
  slug: ezyvet-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-prescriptions-api-openapi.yml
- filename: ezyvet-products-api-openapi.yml
  format: yaml
  label: ezyVet Products API
  slug: ezyvet-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-products-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ezyvet Authentication
name_suffix: Authentication
oauth_flows: []
overview: ezyVet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ezyVet
provider_slug: ezyvet
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token from POST /v1/oauth/access_token (OAuth 2.0 Client Credentials). 12-hour TTL.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ezyvet-openapi.yml
  type: http
slug: ezyvet-authentication
source_filename: ezyvet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ezyvet-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token from POST /v1/oauth/access_token (OAuth 2.0 Client Credentials).\n    12-hour TTL.\n  sources:\n  - openapi/ezyvet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/authentication/ezyvet-authentication.yml
summary_line: http · 1 scheme
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- Animal Health
- IDEXX
- Partner Gated
---
