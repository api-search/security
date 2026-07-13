---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Splitit Installments API v3
  slug: splitit-installments-api-v3
  spec_type: OpenAPI
  url: https://developers.splitit.com/api/v3/introduction/
- filename: splitit-account-management-api.yml
  format: yaml
  label: Splitit Account Management System API
  slug: splitit-account-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/openapi/splitit-account-management-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Splitit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Splitit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Splitit
provider_slug: splitit
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/splitit-account-management-api.yml
  - openapi/splitit-installments-api-v3.yml
  type: http
slug: splitit-authentication
source_filename: splitit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/splitit-account-management-api.yml, openapi/splitit-installments-api-v3.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/splitit-account-management-api.yml\n  - openapi/splitit-installments-api-v3.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/authentication/splitit-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Installments
- Buy Now Pay Later
- Credit Card
- Fintech
- E-commerce
---
