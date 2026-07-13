---
api_key_in:
- header
api_specs:
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Products API
  slug: tiendanube-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Product Variants API
  slug: tiendanube-product-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Categories API
  slug: tiendanube-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Orders API
  slug: tiendanube-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Customers API
  slug: tiendanube-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Coupons API
  slug: tiendanube-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Webhooks API
  slug: tiendanube-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Scripts API
  slug: tiendanube-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Fulfillment Orders API
  slug: tiendanube-fulfillment-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
- filename: tiendanube-openapi.yml
  format: yaml
  label: Tiendanube Payment and Shipping Providers API
  slug: tiendanube-payment-shipping-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tiendanube Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tiendanube secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tiendanube
provider_slug: tiendanube
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token obtained via the authorization-code flow, sent as "Authentication: bearer {access_token}". A descriptive User-Agent header is also required on every request.'
  in: header
  name: AuthenticationToken
  parameter: Authentication
  sources:
  - openapi/tiendanube-openapi.yml
  type: apiKey
slug: tiendanube-authentication
source_filename: tiendanube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tiendanube-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthenticationToken\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: 'OAuth 2.0 access token obtained via the authorization-code flow, sent as \"Authentication:\n    bearer {access_token}\". A descriptive User-Agent header is also required on every request.'\n  sources:\n  - openapi/tiendanube-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/authentication/tiendanube-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-commerce
- Retail
- Latin America
- Storefront
- Products
- Orders
---
