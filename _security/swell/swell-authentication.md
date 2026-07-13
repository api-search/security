---
api_key_in: []
api_specs:
- filename: swell-openapi.yml
  format: yaml
  label: Swell Backend API
  slug: backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swell/refs/heads/main/openapi/swell-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Swell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swell secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swell
provider_slug: swell
scheme_count: 1
schemes:
- description: HTTP Basic auth where the username is your Swell Store ID and the password is your Secret Key from the Developer dashboard.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/swell-openapi.yml
  type: http
slug: swell-authentication
source_filename: swell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swell-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth where the username is your Swell Store ID and the password is\n    your Secret Key from the Developer dashboard.\n  sources:\n  - openapi/swell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swell/refs/heads/main/authentication/swell-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- Ecommerce
- Storefront
- Subscriptions
- B2B
- Products
- Orders
- Customers
---
