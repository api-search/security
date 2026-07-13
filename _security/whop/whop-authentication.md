---
api_key_in: []
api_specs:
- filename: whop-openapi.yml
  format: yaml
  label: Whop Memberships API
  slug: whop-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Products API
  slug: whop-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Plans API
  slug: whop-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Payments API
  slug: whop-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Users API
  slug: whop-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Companies API
  slug: whop-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Checkout Configurations API
  slug: whop-checkout-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Transfers API
  slug: whop-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Webhooks API
  slug: whop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Promo Codes API
  slug: whop-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-asyncapi.yml
  format: yaml
  label: Whop Realtime WebSocket API
  slug: whop-realtime-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/asyncapi/whop-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Whop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Whop
provider_slug: whop
scheme_count: 1
schemes:
- bearerFormat: Whop API key
  description: 'Bearer token authentication. Use a Company/Account API key or an App API key in the `Authorization: Bearer <API_KEY>` header. OAuth access tokens are used when acting on behalf of a signed-in Whop user.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/whop-openapi.yml
  type: http
slug: whop-authentication
source_filename: whop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whop-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Whop API key\n  description: 'Bearer token authentication. Use a Company/Account API key or an App API key\n    in the `Authorization: Bearer <API_KEY>` header. OAuth access tokens are used when acting\n    on behalf of a signed-in Whop user.'\n  sources:\n  - openapi/whop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/authentication/whop-authentication.yml
summary_line: http · 1 scheme
tags:
- Memberships
- Payments
- Creator Economy
- Marketplace
- Digital Products
- Access Control
- Commerce
---
