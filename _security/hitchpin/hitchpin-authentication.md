---
api_key_in:
- cookie
- header
api_specs:
- filename: hitchpin-django-api-openapi.json
  format: json
  label: HitchPin Django API (Instant Invoicing)
  slug: hitchpin-django-api-instant-invoicing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-django-api-openapi.json
- filename: hitchpin-receipt-rendering-openapi.json
  format: json
  label: HitchPin Receipt Rendering Service
  slug: hitchpin-receipt-rendering-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-receipt-rendering-openapi.json
- filename: hitchpin-url-shortener-openapi.json
  format: json
  label: HitchPin URL Shortcode Service
  slug: hitchpin-url-shortcode-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-url-shortener-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hitchpin Authentication
name_suffix: Authentication
oauth_flows: []
overview: HitchPin secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HitchPin
provider_slug: hitchpin
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/hitchpin-django-api-openapi.json
  type: apiKey
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/hitchpin-django-api-openapi.json
  type: apiKey
slug: hitchpin-authentication
source_filename: hitchpin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hitchpin-django-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/hitchpin-django-api-openapi.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/hitchpin-django-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/authentication/hitchpin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Marketplace
- Agriculture
- Livestock
- Hay and Forage
- Farm Equipment
- Invoicing
- Payments
- Rural
---
