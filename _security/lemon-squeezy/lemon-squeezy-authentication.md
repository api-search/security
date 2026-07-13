---
api_key_in: []
api_specs:
- filename: lemon-squeezy-api-openapi.yml
  format: yaml
  label: Lemon Squeezy API
  slug: lemon-squeezy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemon-squeezy/refs/heads/main/openapi/lemon-squeezy-api-openapi.yml
- filename: lemon-squeezy-license-api-openapi.yml
  format: yaml
  label: Lemon Squeezy License API
  slug: lemon-squeezy-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemon-squeezy/refs/heads/main/openapi/lemon-squeezy-license-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lemon Squeezy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lemon Squeezy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lemon Squeezy
provider_slug: lemon-squeezy
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lemon-squeezy-api-openapi.yml
  type: http
slug: lemon-squeezy-authentication
source_filename: lemon-squeezy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lemon-squeezy-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lemon-squeezy-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-squeezy/refs/heads/main/authentication/lemon-squeezy-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Products
- Ecommerce
- Products
---
