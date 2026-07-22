---
api_key_in: []
api_specs:
- filename: zalando-orders-openapi.yml
  format: yaml
  label: zDirect Platform Orders API
  slug: zalando-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-orders-openapi.yml
- filename: zalando-products-openapi.yml
  format: yaml
  label: zDirect Platform Products API
  slug: zalando-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-products-openapi.yml
- filename: zalando-product-attributes-openapi.yml
  format: yaml
  label: Merchant Product Attributes API
  slug: zalando-product-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-product-attributes-openapi.yml
- filename: zalando-article-requirements-openapi.yml
  format: yaml
  label: Article Requirements API
  slug: zalando-article-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-article-requirements-openapi.yml
- filename: zalando-prices-openapi.yml
  format: yaml
  label: Merchant Price Service API
  slug: zalando-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-prices-openapi.yml
- filename: zalando-price-reporting-openapi.yml
  format: yaml
  label: Price Reporting API
  slug: zalando-price-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-price-reporting-openapi.yml
- filename: zalando-stocks-openapi.yml
  format: yaml
  label: Merchant Stock Service API
  slug: zalando-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-stocks-openapi.yml
- filename: zalando-offer-blocking-openapi.yml
  format: yaml
  label: Article Availability (Offer Blocking) API
  slug: zalando-offer-blocking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-offer-blocking-openapi.yml
- filename: zalando-sales-channels-openapi.yml
  format: yaml
  label: Sales Channels API
  slug: zalando-sales-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-sales-channels-openapi.yml
- filename: zalando-logistic-centers-openapi.yml
  format: yaml
  label: Logistic Centers API
  slug: zalando-logistic-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-logistic-centers-openapi.yml
- filename: zalando-zfs-stock-movements-openapi.yml
  format: yaml
  label: ZFS Stock Movements API
  slug: zalando-zfs-stock-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-stock-movements-openapi.yml
- filename: zalando-zfs-cross-border-movements-openapi.yml
  format: yaml
  label: ZFS Cross-Border Movements Report API
  slug: zalando-zfs-cross-border-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-cross-border-movements-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zalando Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zalando secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zalando
provider_slug: zalando
scheme_count: 1
schemes:
- description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth 2 to handle the client credentials process flow.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  sources:
  - openapi/zalando-logistic-centers-openapi.yml
  - openapi/zalando-offer-blocking-openapi.yml
  - openapi/zalando-orders-openapi.yml
  - openapi/zalando-price-reporting-openapi.yml
  - openapi/zalando-prices-openapi.yml
  - openapi/zalando-product-attributes-openapi.yml
  - openapi/zalando-products-openapi.yml
  - openapi/zalando-sales-channels-openapi.yml
  - openapi/zalando-stocks-openapi.yml
  - openapi/zalando-zfs-cross-border-movements-openapi.yml
  - openapi/zalando-zfs-stock-movements-openapi.yml
  type: oauth2
slug: zalando-authentication
source_filename: zalando-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zalando-logistic-centers-openapi.yml, openapi/zalando-offer-blocking-openapi.yml,\n  openapi/zalando-orders-openapi.yml, openapi/zalando-price-reporting-openapi.yml, openapi/zalando-prices-openapi.yml,\n  openapi/zalando-product-attributes-openapi.yml, openapi/zalando-products-openapi.yml, openapi/zalando-sales-channels-openapi.yml,\n  openapi/zalando-stocks-openapi.yml, openapi/zalando-zfs-cross-border-movements-openapi.yml,\n  openapi/zalando-zfs-stock-movements-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: merchant_platform\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.merchants.zalando.com/auth/token\n    scopes: 1\n  description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth\n    2 to handle the client credentials process flow.\n  sources:\n  - openapi/zalando-logistic-centers-openapi.yml\n\
  \  - openapi/zalando-offer-blocking-openapi.yml\n  - openapi/zalando-orders-openapi.yml\n  - openapi/zalando-price-reporting-openapi.yml\n  - openapi/zalando-prices-openapi.yml\n  - openapi/zalando-product-attributes-openapi.yml\n  - openapi/zalando-products-openapi.yml\n  - openapi/zalando-sales-channels-openapi.yml\n  - openapi/zalando-stocks-openapi.yml\n  - openapi/zalando-zfs-cross-border-movements-openapi.yml\n  - openapi/zalando-zfs-stock-movements-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/authentication/zalando-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer; Marketplace
- Fashion
- E-Commerce
- Retail
- Marketplace
- Fulfillment
- Merchant Platform
- Orders
- Products
---
