---
api_key_in: []
api_specs:
- filename: otter-account-pairing-endpoints-api-openapi.yml
  format: yaml
  label: Otter Account Pairing Endpoints API
  slug: otter-account-pairing-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-account-pairing-endpoints-api-openapi.yml
- filename: otter-auth-endpoints-api-openapi.yml
  format: yaml
  label: Otter Auth Endpoints API
  slug: otter-auth-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-auth-endpoints-api-openapi.yml
- filename: otter-callback-endpoints-api-openapi.yml
  format: yaml
  label: Otter Callback Endpoints API
  slug: otter-callback-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-callback-endpoints-api-openapi.yml
- filename: otter-delivery-endpoints-api-openapi.yml
  format: yaml
  label: Otter Delivery Endpoints API
  slug: otter-delivery-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-delivery-endpoints-api-openapi.yml
- filename: otter-direct-orders-endpoints-api-openapi.yml
  format: yaml
  label: Otter Direct Orders Endpoints API
  slug: otter-direct-orders-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-direct-orders-endpoints-api-openapi.yml
- filename: otter-finance-endpoints-api-openapi.yml
  format: yaml
  label: Otter Finance Endpoints API
  slug: otter-finance-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-finance-endpoints-api-openapi.yml
- filename: otter-inventory-endpoints-api-openapi.yml
  format: yaml
  label: Otter Inventory Endpoints API
  slug: otter-inventory-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-inventory-endpoints-api-openapi.yml
- filename: otter-manager-loyalty-endpoints-api-openapi.yml
  format: yaml
  label: Otter Manager Loyalty Endpoints API
  slug: otter-manager-loyalty-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-manager-loyalty-endpoints-api-openapi.yml
- filename: otter-manager-menu-endpoints-api-openapi.yml
  format: yaml
  label: Otter Manager Menu Endpoints API
  slug: otter-manager-menu-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-manager-menu-endpoints-api-openapi.yml
- filename: otter-manager-order-endpoints-api-openapi.yml
  format: yaml
  label: Otter Manager Order Endpoints API
  slug: otter-manager-order-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-manager-order-endpoints-api-openapi.yml
- filename: otter-manager-storefront-endpoints-api-openapi.yml
  format: yaml
  label: Otter Manager Storefront Endpoints API
  slug: otter-manager-storefront-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-manager-storefront-endpoints-api-openapi.yml
- filename: otter-market-intel-endpoints-api-openapi.yml
  format: yaml
  label: Otter Market Intel Endpoints API
  slug: otter-market-intel-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-market-intel-endpoints-api-openapi.yml
- filename: otter-menus-endpoints-api-openapi.yml
  format: yaml
  label: Otter Menus Endpoints API
  slug: otter-menus-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-menus-endpoints-api-openapi.yml
- filename: otter-orders-endpoints-api-openapi.yml
  format: yaml
  label: Otter Orders Endpoints API
  slug: otter-orders-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-orders-endpoints-api-openapi.yml
- filename: otter-organization-endpoints-api-openapi.yml
  format: yaml
  label: Otter Organization Endpoints API
  slug: otter-organization-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-organization-endpoints-api-openapi.yml
- filename: otter-ping-endpoints-api-openapi.yml
  format: yaml
  label: Otter Ping Endpoints API
  slug: otter-ping-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-ping-endpoints-api-openapi.yml
- filename: otter-reports-endpoints-api-openapi.yml
  format: yaml
  label: Otter Reports Endpoints API
  slug: otter-reports-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-reports-endpoints-api-openapi.yml
- filename: otter-reviews-endpoints-api-openapi.yml
  format: yaml
  label: Otter Reviews Endpoints API
  slug: otter-reviews-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-reviews-endpoints-api-openapi.yml
- filename: otter-storefront-endpoints-api-openapi.yml
  format: yaml
  label: Otter Storefront Endpoints API
  slug: otter-storefront-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-storefront-endpoints-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Otter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Otter secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Otter
provider_slug: otter
scheme_count: 1
schemes:
- description: 'The **Authorization API** is based on the [OAuth2.0 protocol](https://tools.ietf.org/html/rfc6749), supporting the (Client Credentials)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.4] and the (Authorization Code)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.1] flows. Resources expect a valid token sent as a `Bearer` token in the HTTP `Authorization` header.

    ### Scopes

    Scopes '
  flows:
  - flow: clientCredentials
    scopes: 27
    tokenUrl: /v1/auth/token
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: /v1/auth/token
  name: OAuth2.0
  sources:
  - openapi/otter-public-api-openapi.yml
  type: oauth2
slug: otter-authentication
source_filename: otter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/otter-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2.0\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n    scopes: 27\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/token\n    scopes: 2\n  description: \"The **Authorization API** is based on the [OAuth2.0 protocol](https://tools.ietf.org/html/rfc6749),\\\n    \\ supporting the (Client Credentials)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.4]\\\n    \\ and the (Authorization Code)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.1]\\\n    \\ flows. Resources expect a valid token sent as a `Bearer` token in the HTTP `Authorization`\\\n    \\ header.\\n### Scopes\\nScopes \"\n  sources:\n  - openapi/otter-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/authentication/otter-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Restaurant
- Order Management
- Delivery
- Online Ordering
- Menu Management
- Analytics
---
