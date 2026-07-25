---
api_key_in: []
api_specs:
- filename: nuvemshop-categories-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Categories API
  slug: nuvemshop-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-categories-api-openapi.yml
- filename: nuvemshop-coupons-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Coupons API
  slug: nuvemshop-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-coupons-api-openapi.yml
- filename: nuvemshop-customers-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Customers API
  slug: nuvemshop-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-customers-api-openapi.yml
- filename: nuvemshop-orders-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Orders API
  slug: nuvemshop-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-orders-api-openapi.yml
- filename: nuvemshop-product-images-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Product Images API
  slug: nuvemshop-product-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-product-images-api-openapi.yml
- filename: nuvemshop-product-variants-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Product Variants API
  slug: nuvemshop-product-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-product-variants-api-openapi.yml
- filename: nuvemshop-products-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Products API
  slug: nuvemshop-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-products-api-openapi.yml
- filename: nuvemshop-scripts-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Scripts API
  slug: nuvemshop-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-scripts-api-openapi.yml
- filename: nuvemshop-store-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Store API
  slug: nuvemshop-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-store-api-openapi.yml
- filename: nuvemshop-webhooks-api-openapi.yml
  format: yaml
  label: Nuvemshop / Tiendanube Webhooks API
  slug: nuvemshop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/openapi/nuvemshop-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Nuvemshop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuvemshop / Tiendanube secures its APIs with apiKey and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nuvemshop / Tiendanube
provider_slug: nuvemshop
scheme_count: 1
schemes:
- description: 'NON-STANDARD auth header. Nuvemshop / Tiendanube apps authenticate with OAuth 2 (authorization code grant) and receive a NON-EXPIRING access token. That token is sent on every request in a header named `Authentication` (not `Authorization`) with a lowercase `bearer` prefix: `Authentication: bearer ACCESS_TOKEN`. Using `Authorization`, an uppercase `Bearer`, or any other casing returns 401. A descriptive `User-Agent` header identifying the app and a contact (e.g. `MyApp (name@email.com)`) is also REQUIRED on every request; omitting it returns 400.'
  headerName: Authentication
  in: header
  name: authenticationHeader
  sources:
  - openapi/nuvemshop-openapi.yml
  - https://tiendanube.github.io/api-documentation/intro
  - https://tiendanube.github.io/api-documentation/authentication
  type: apiKey
slug: nuvemshop-authentication
source_filename: nuvemshop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/nuvemshop-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\nschemes:\n- name: authenticationHeader\n  type: apiKey\n  in: header\n  headerName: Authentication\n  description: >-\n    NON-STANDARD auth header. Nuvemshop / Tiendanube apps authenticate with\n    OAuth 2 (authorization code grant) and receive a NON-EXPIRING access token.\n    That token is sent on every request in a header named `Authentication`\n    (not `Authorization`) with a lowercase `bearer` prefix:\n    `Authentication: bearer ACCESS_TOKEN`. Using `Authorization`, an uppercase\n    `Bearer`, or any other casing returns 401. A descriptive `User-Agent`\n    header identifying the app and a contact (e.g. `MyApp (name@email.com)`) is\n    also REQUIRED on every request; omitting it returns 400.\n  sources:\n  - openapi/nuvemshop-openapi.yml\n  - https://tiendanube.github.io/api-documentation/intro\n  - https://tiendanube.github.io/api-documentation/authentication\n\
  oauth2:\n  grantTypes:\n  - authorization_code\n  authorizationUrl: https://www.tiendanube.com/apps/{app_id}/authorize\n  tokenUrl: https://www.tiendanube.com/apps/authorize/token\n  tokenExpiry: non-expiring\n  notes: >-\n    The authorization URL takes a `state` (CSRF) parameter. The token exchange\n    is a POST to https://www.tiendanube.com/apps/authorize/token with a JSON\n    body of client_id, client_secret, grant_type=authorization_code, and the\n    authorization code. The response returns access_token, token_type \"bearer\",\n    the granted scope, and user_id (the numeric store id used in every API\n    path). The nuvemshop.com.br domain mirrors the same endpoints for Brazil.\n  scopesNote: >-\n    Scopes are granted per app and appear in the token response `scope` field\n    (for example read_products, write_products, read_orders, write_orders,\n    read_customers, write_customers, read_coupons, write_coupons,\n    read_scripts, write_scripts).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvemshop/refs/heads/main/authentication/nuvemshop-authentication.yml
summary_line: apiKey/oauth2 · 1 scheme
tags:
- E-commerce
- Online Store
- Latin America
- Brazil
- Argentina
- Storefront
- Products
- Orders
- Merchants
- Webhooks
- SaaS
---
