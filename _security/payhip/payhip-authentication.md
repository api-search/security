---
api_key_in:
- header
api_specs:
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip Coupons API
  slug: payhip-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip License Keys API
  slug: payhip-license-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip Webhooks API
  slug: payhip-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Payhip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payhip secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Payhip
provider_slug: payhip
scheme_count: 2
schemes:
- description: Account API key from the Developer Settings page. Used for coupon operations.
  in: header
  name: apiKeyAuth
  parameter: payhip-api-key
  sources:
  - openapi/payhip-openapi.yml
  type: apiKey
- description: Per-product secret key from the Developer Settings page. Used for license key operations.
  in: header
  name: productSecretAuth
  parameter: product-secret-key
  sources:
  - openapi/payhip-openapi.yml
  type: apiKey
slug: payhip-authentication
source_filename: payhip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/payhip-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: payhip-api-key\n  description: Account API key from the Developer Settings page. Used for coupon operations.\n  sources:\n  - openapi/payhip-openapi.yml\n- name: productSecretAuth\n  type: apiKey\n  in: header\n  parameter: product-secret-key\n  description: Per-product secret key from the Developer Settings page. Used for license key\n    operations.\n  sources:\n  - openapi/payhip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/authentication/payhip-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- E-commerce
- Digital Products
- Memberships
- Creators
- Coupons
- License Keys
- Webhooks
- Payments
---
