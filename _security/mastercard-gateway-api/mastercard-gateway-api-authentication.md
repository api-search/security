---
api_key_in: []
api_specs:
- filename: mastercard-gateway-api-openapi.yml
  format: yaml
  label: Mastercard Gateway API
  slug: mastercard-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-gateway-api/refs/heads/main/openapi/mastercard-gateway-api-openapi.yml
auth_types:
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Mastercard Gateway Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mastercard Gateway API secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mastercard Gateway API
provider_slug: mastercard-gateway-api
scheme_count: 2
schemes:
- description: 'HTTP Basic authentication using `merchant.<merchantId>` as the

    username and the API password (integration password) as the

    password.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/mastercard-gateway-api-openapi.yml
  type: http
- description: 'Client-certificate (mutual TLS) authentication, available as an

    alternative to password-based merchant authentication.'
  name: CertificateAuth
  sources:
  - openapi/mastercard-gateway-api-openapi.yml
  type: mutualTLS
slug: mastercard-gateway-api-authentication
source_filename: mastercard-gateway-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mastercard-gateway-api-openapi.yml\nsummary:\n  types:\n  - http\n  - mutualTLS\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic authentication using `merchant.<merchantId>` as the\n    username and the API password (integration password) as the\n    password.\n  sources:\n  - openapi/mastercard-gateway-api-openapi.yml\n- name: CertificateAuth\n  type: mutualTLS\n  description: |-\n    Client-certificate (mutual TLS) authentication, available as an\n    alternative to password-based merchant authentication.\n  sources:\n  - openapi/mastercard-gateway-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercard-gateway-api/refs/heads/main/authentication/mastercard-gateway-api-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- Credit Cards
- Gateway
- Payment Processing
- Payments
---
