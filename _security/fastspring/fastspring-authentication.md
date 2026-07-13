---
api_key_in: []
api_specs:
- filename: fastspring-openapi.yml
  format: yaml
  label: FastSpring API
  slug: commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fastspring Authentication
name_suffix: Authentication
oauth_flows: []
overview: FastSpring secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FastSpring
provider_slug: fastspring
scheme_count: 1
schemes:
- description: HTTP Basic with credentials from FastSpring App Dashboard
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/fastspring-openapi.yml
  type: http
slug: fastspring-authentication
source_filename: fastspring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fastspring-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with credentials from FastSpring App Dashboard\n  sources:\n  - openapi/fastspring-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/authentication/fastspring-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Merchant of Record
- Subscription Billing
- Payments
- SaaS Billing
- Checkout
- Tax Compliance
---
