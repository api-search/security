---
api_key_in: []
api_specs:
- filename: flipdish-apps-openapi.json
  format: json
  label: Flipdish Apps & Channels API
  slug: apps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-apps-openapi.json
- filename: flipdish-catalog-openapi.json
  format: json
  label: Flipdish Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-catalog-openapi.json
- filename: flipdish-customers-openapi.json
  format: json
  label: Flipdish Customers & Accounts API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-customers-openapi.json
- filename: flipdish-devices-openapi.json
  format: json
  label: Flipdish Devices API
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-devices-openapi.json
- filename: flipdish-marketing-openapi.json
  format: json
  label: Flipdish Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-marketing-openapi.json
- filename: flipdish-menus-openapi.json
  format: json
  label: Flipdish Menus API
  slug: menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-menus-openapi.json
- filename: flipdish-orders-openapi.json
  format: json
  label: Flipdish Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-orders-openapi.json
- filename: flipdish-payments-openapi.json
  format: json
  label: Flipdish Payments & Payouts API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-payments-openapi.json
- filename: flipdish-platform-openapi.json
  format: json
  label: Flipdish Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-platform-openapi.json
- filename: flipdish-stores-openapi.json
  format: json
  label: Flipdish Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-stores-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Flipdish Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- implicit
overview: Flipdish secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and implicit flow(s).
provider_name: Flipdish
provider_slug: flipdish
scheme_count: 1
schemes:
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
    scopes: 1
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  sources:
  - openapi/flipdish-apps-openapi.json
  - openapi/flipdish-catalog-openapi.json
  - openapi/flipdish-customers-openapi.json
  - openapi/flipdish-devices-openapi.json
  - openapi/flipdish-marketing-openapi.json
  - openapi/flipdish-menus-openapi.json
  - openapi/flipdish-orders-openapi.json
  - openapi/flipdish-payments-openapi.json
  - openapi/flipdish-platform-openapi.json
  - openapi/flipdish-stores-openapi.json
  type: oauth2
slug: flipdish-authentication
source_filename: flipdish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flipdish-apps-openapi.json, openapi/flipdish-catalog-openapi.json, openapi/flipdish-customers-openapi.json,\n  openapi/flipdish-devices-openapi.json, openapi/flipdish-marketing-openapi.json, openapi/flipdish-menus-openapi.json,\n  openapi/flipdish-orders-openapi.json, openapi/flipdish-payments-openapi.json, openapi/flipdish-platform-openapi.json,\n  openapi/flipdish-stores-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n    scopes: 1\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n\
  \    token).\n  sources:\n  - openapi/flipdish-apps-openapi.json\n  - openapi/flipdish-catalog-openapi.json\n  - openapi/flipdish-customers-openapi.json\n  - openapi/flipdish-devices-openapi.json\n  - openapi/flipdish-marketing-openapi.json\n  - openapi/flipdish-menus-openapi.json\n  - openapi/flipdish-orders-openapi.json\n  - openapi/flipdish-payments-openapi.json\n  - openapi/flipdish-platform-openapi.json\n  - openapi/flipdish-stores-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/authentication/flipdish-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Restaurant
- Online Ordering
- Mobile Apps
- Point of Sale
- Orders
- Menu
- Payments
- Webhooks
---
