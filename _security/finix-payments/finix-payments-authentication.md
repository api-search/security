---
api_key_in: []
api_specs:
- filename: finix-payments-openapi-original.yml
  format: yaml
  label: Finix API
  slug: finix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix-payments/refs/heads/main/openapi/finix-payments-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Finix Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finix Payments secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finix Payments
provider_slug: finix-payments
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/finix-payments-openapi-original.yml
  type: http
slug: finix-payments-authentication
source_filename: finix-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/finix-payments-openapi-original.yml\ndocs: https://docs.finix.com/additional-resources/developers/authentication-and-api-basics/api-keys\ndetail: >-\n  Finix authenticates every request with HTTP Basic Authentication (RFC 7617). The username is the API Key\n  id (e.g. USxxxxxxxx) and the password is the API Key secret; combine as \"username:password\", Base64-encode,\n  and send as Authorization: Basic <base64>. API Keys are created in the Finix Dashboard and are environment\n  scoped — Sandbox keys cannot be used in Live and vice-versa. There is no OAuth2/OIDC surface.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/finix-payments-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finix-payments/refs/heads/main/authentication/finix-payments-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Payment Processing
- Payment Facilitation
- Embedded Finance
- Marketplaces
- ACH
- Card Acceptance
- Fintech
- PCI DSS
---
