---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Przelewy24 REST API
  slug: przelewy24-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi.yml
- filename: openapi-marketplace.yml
  format: yaml
  label: Przelewy24 Marketplace API
  slug: przelewy24-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/openapi-marketplace.yml
- filename: openapi-extended.yml
  format: yaml
  label: Przelewy24 Extended API
  slug: przelewy24-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/openapi-extended.yml
- filename: openapi-ekspres.yml
  format: yaml
  label: Przelewy24 Ekspres API
  slug: przelewy24-ekspres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/openapi-ekspres.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Przelewy24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Przelewy24 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Przelewy24
provider_slug: przelewy24
scheme_count: 1
schemes:
- description: This is the default authentication method. User login is API REST key the password assigned to it.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/openapi-ekspres.yml
  - openapi/openapi-extended.yml
  - openapi/openapi-marketplace.yml
  - openapi/openapi.yml
  type: http
slug: przelewy24-authentication
source_filename: przelewy24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi-ekspres.yml, openapi/openapi-extended.yml, openapi/openapi-marketplace.yml,\n  openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: This is the default authentication method. User login is API REST key the password\n    assigned to it.\n  sources:\n  - openapi/openapi-ekspres.yml\n  - openapi/openapi-extended.yml\n  - openapi/openapi-marketplace.yml\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/authentication/przelewy24-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Gateway
- Bank Transfer
- BLIK
- Card Payments
- E-Commerce
- Poland
- Polish
- Multi-Currency
- Fintech
---
