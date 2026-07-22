---
api_key_in: []
api_specs:
- filename: resolve-merchant-api-openapi.yaml
  format: yaml
  label: Resolve Merchant API
  slug: resolve-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-merchant-api-openapi.yaml
- filename: resolve-partners-api-openapi.yaml
  format: yaml
  label: Resolve Partners API
  slug: resolve-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-partners-api-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Resolve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Resolve secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Resolve
provider_slug: resolve
scheme_count: 2
schemes:
- description: HTTP Basic Auth using `merchant_id` as username and the merchant secret key as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/resolve-merchant-api-openapi.yaml
  - openapi/resolve-partners-api-openapi.yaml
  type: http
- bearerFormat: JWT
  description: Bearer token authentication using an OAuth access token minted for an API access key created in Merchant Dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/resolve-merchant-api-openapi.yaml
  - openapi/resolve-partners-api-openapi.yaml
  type: http
slug: resolve-authentication
source_filename: resolve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/resolve-merchant-api-openapi.yaml, openapi/resolve-partners-api-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using `merchant_id` as username and the merchant secret key as\n    password.\n  sources:\n  - openapi/resolve-merchant-api-openapi.yaml\n  - openapi/resolve-partners-api-openapi.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication using an OAuth access token minted for an API access\n    key created in Merchant Dashboard.\n  sources:\n  - openapi/resolve-merchant-api-openapi.yaml\n  - openapi/resolve-partners-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/authentication/resolve-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Payments
- B2B
- Net Terms
- Credit
- Invoicing
- Financing
- Embedded Finance
---
