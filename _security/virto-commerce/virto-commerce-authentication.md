---
api_key_in:
- header
- query
api_specs:
- filename: VirtoCommerce.Catalog
  format: yaml
  label: Virto Commerce Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Catalog
- filename: VirtoCommerce.Pricing
  format: yaml
  label: Virto Commerce Pricing API
  slug: pricing
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Pricing
- filename: VirtoCommerce.Inventory
  format: yaml
  label: Virto Commerce Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Inventory
- filename: VirtoCommerce.Orders
  format: yaml
  label: Virto Commerce Order Management API
  slug: orders
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Orders
- filename: VirtoCommerce.Cart
  format: yaml
  label: Virto Commerce Shopping Cart API
  slug: cart
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Cart
- filename: VirtoCommerce.Customer
  format: yaml
  label: Virto Commerce Customer API
  slug: customer
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Customer
- filename: VirtoCommerce.Marketing
  format: yaml
  label: Virto Commerce Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Marketing
- filename: VirtoCommerce.Quote
  format: yaml
  label: Virto Commerce Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Quote
- filename: VirtoCommerce.Store
  format: yaml
  label: Virto Commerce Store API
  slug: store
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Store
- filename: VirtoCommerce.Platform
  format: yaml
  label: Virto Commerce Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Platform
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Virto Commerce Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Virto Commerce secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Virto Commerce
provider_slug: virto-commerce
scheme_count: 5
schemes:
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    scopes: 0
    tokenUrl: /connect/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /connect/token
  name: oauth2
  sources:
  - openapi/virto-commerce-cart-openapi.json
  - openapi/virto-commerce-catalog-openapi.json
  - openapi/virto-commerce-customer-openapi.json
  - openapi/virto-commerce-inventory-openapi.json
  - openapi/virto-commerce-marketing-openapi.json
  - openapi/virto-commerce-orders-openapi.json
  - openapi/virto-commerce-platform-openapi.json
  - openapi/virto-commerce-pricing-openapi.json
  - openapi/virto-commerce-quote-openapi.json
  - openapi/virto-commerce-store-openapi.json
  type: oauth2
- description: API Key authentication
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/virto-commerce-cart-openapi.json
  - openapi/virto-commerce-catalog-openapi.json
  - openapi/virto-commerce-customer-openapi.json
  - openapi/virto-commerce-inventory-openapi.json
  - openapi/virto-commerce-marketing-openapi.json
  - openapi/virto-commerce-orders-openapi.json
  - openapi/virto-commerce-platform-openapi.json
  - openapi/virto-commerce-pricing-openapi.json
  - openapi/virto-commerce-quote-openapi.json
  - openapi/virto-commerce-store-openapi.json
  type: apiKey
- description: API Key authentication (alternative via header)
  in: header
  name: api_key_header
  parameter: api_key
  sources:
  - openapi/virto-commerce-cart-openapi.json
  - openapi/virto-commerce-catalog-openapi.json
  - openapi/virto-commerce-customer-openapi.json
  - openapi/virto-commerce-inventory-openapi.json
  - openapi/virto-commerce-marketing-openapi.json
  - openapi/virto-commerce-orders-openapi.json
  - openapi/virto-commerce-platform-openapi.json
  - openapi/virto-commerce-pricing-openapi.json
  - openapi/virto-commerce-quote-openapi.json
  - openapi/virto-commerce-store-openapi.json
  type: apiKey
- description: HTTP Signature authentication using Authorization header
  name: http-signature
  scheme: signature
  sources:
  - openapi/virto-commerce-cart-openapi.json
  - openapi/virto-commerce-catalog-openapi.json
  - openapi/virto-commerce-customer-openapi.json
  - openapi/virto-commerce-inventory-openapi.json
  - openapi/virto-commerce-marketing-openapi.json
  - openapi/virto-commerce-orders-openapi.json
  - openapi/virto-commerce-platform-openapi.json
  - openapi/virto-commerce-pricing-openapi.json
  - openapi/virto-commerce-quote-openapi.json
  - openapi/virto-commerce-store-openapi.json
  type: http
- description: Basic authentication using username and password
  name: basic
  scheme: basic
  sources:
  - openapi/virto-commerce-cart-openapi.json
  - openapi/virto-commerce-catalog-openapi.json
  - openapi/virto-commerce-customer-openapi.json
  - openapi/virto-commerce-inventory-openapi.json
  - openapi/virto-commerce-marketing-openapi.json
  - openapi/virto-commerce-orders-openapi.json
  - openapi/virto-commerce-platform-openapi.json
  - openapi/virto-commerce-pricing-openapi.json
  - openapi/virto-commerce-quote-openapi.json
  - openapi/virto-commerce-store-openapi.json
  type: http
slug: virto-commerce-authentication
source_filename: virto-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/virto-commerce-cart-openapi.json, openapi/virto-commerce-catalog-openapi.json,\n  openapi/virto-commerce-customer-openapi.json, openapi/virto-commerce-inventory-openapi.json,\n  openapi/virto-commerce-marketing-openapi.json, openapi/virto-commerce-orders-openapi.json,\n  openapi/virto-commerce-platform-openapi.json, openapi/virto-commerce-pricing-openapi.json,\n  openapi/virto-commerce-quote-openapi.json, openapi/virto-commerce-store-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n    scopes: 0\n  description: OAuth2 Resource Owner Password Grant flow\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n  - openapi/virto-commerce-catalog-openapi.json\n\
  \  - openapi/virto-commerce-customer-openapi.json\n  - openapi/virto-commerce-inventory-openapi.json\n  - openapi/virto-commerce-marketing-openapi.json\n  - openapi/virto-commerce-orders-openapi.json\n  - openapi/virto-commerce-platform-openapi.json\n  - openapi/virto-commerce-pricing-openapi.json\n  - openapi/virto-commerce-quote-openapi.json\n  - openapi/virto-commerce-store-openapi.json\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API Key authentication\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n  - openapi/virto-commerce-catalog-openapi.json\n  - openapi/virto-commerce-customer-openapi.json\n  - openapi/virto-commerce-inventory-openapi.json\n  - openapi/virto-commerce-marketing-openapi.json\n  - openapi/virto-commerce-orders-openapi.json\n  - openapi/virto-commerce-platform-openapi.json\n  - openapi/virto-commerce-pricing-openapi.json\n  - openapi/virto-commerce-quote-openapi.json\n  - openapi/virto-commerce-store-openapi.json\n\
  - name: api_key_header\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: API Key authentication (alternative via header)\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n  - openapi/virto-commerce-catalog-openapi.json\n  - openapi/virto-commerce-customer-openapi.json\n  - openapi/virto-commerce-inventory-openapi.json\n  - openapi/virto-commerce-marketing-openapi.json\n  - openapi/virto-commerce-orders-openapi.json\n  - openapi/virto-commerce-platform-openapi.json\n  - openapi/virto-commerce-pricing-openapi.json\n  - openapi/virto-commerce-quote-openapi.json\n  - openapi/virto-commerce-store-openapi.json\n- name: http-signature\n  type: http\n  scheme: signature\n  description: HTTP Signature authentication using Authorization header\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n  - openapi/virto-commerce-catalog-openapi.json\n  - openapi/virto-commerce-customer-openapi.json\n  - openapi/virto-commerce-inventory-openapi.json\n  - openapi/virto-commerce-marketing-openapi.json\n\
  \  - openapi/virto-commerce-orders-openapi.json\n  - openapi/virto-commerce-platform-openapi.json\n  - openapi/virto-commerce-pricing-openapi.json\n  - openapi/virto-commerce-quote-openapi.json\n  - openapi/virto-commerce-store-openapi.json\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic authentication using username and password\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n  - openapi/virto-commerce-catalog-openapi.json\n  - openapi/virto-commerce-customer-openapi.json\n  - openapi/virto-commerce-inventory-openapi.json\n  - openapi/virto-commerce-marketing-openapi.json\n  - openapi/virto-commerce-orders-openapi.json\n  - openapi/virto-commerce-platform-openapi.json\n  - openapi/virto-commerce-pricing-openapi.json\n  - openapi/virto-commerce-quote-openapi.json\n  - openapi/virto-commerce-store-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/authentication/virto-commerce-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- B2B E-Commerce
- Catalog Management
- Order Management
- Pricing
- Inventory
- Shopping Cart
- Customer Management
- Marketing
- Payments
- Shipping
- Subscriptions
- Headless Commerce
- Open Source
- .NET
---
