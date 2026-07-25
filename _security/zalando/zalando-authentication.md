---
api_key_in: []
api_specs:
- filename: zalando-announcedreturns-api-openapi.yml
  format: yaml
  label: Zalando AnnouncedReturns API
  slug: zalando-announcedreturns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-announcedreturns-api-openapi.yml
- filename: zalando-attribute-types-api-openapi.yml
  format: yaml
  label: Zalando attribute-types API
  slug: zalando-attribute-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-attribute-types-api-openapi.yml
- filename: zalando-attribute-values-api-openapi.yml
  format: yaml
  label: Zalando attribute-values API
  slug: zalando-attribute-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-attribute-values-api-openapi.yml
- filename: zalando-attributes-api-openapi.yml
  format: yaml
  label: Zalando Attributes API
  slug: zalando-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-attributes-api-openapi.yml
- filename: zalando-cross-border-movements-api-openapi.yml
  format: yaml
  label: Zalando Cross Border Movements API
  slug: zalando-cross-border-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-cross-border-movements-api-openapi.yml
- filename: zalando-discovery-api-api-openapi.yml
  format: yaml
  label: Zalando Discovery API API
  slug: zalando-discovery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-discovery-api-api-openapi.yml
- filename: zalando-history-of-price-update-attempts-api-openapi.yml
  format: yaml
  label: Zalando History of Price Update Attempts API
  slug: zalando-history-of-price-update-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-history-of-price-update-attempts-api-openapi.yml
- filename: zalando-liquidated-items-api-openapi.yml
  format: yaml
  label: Zalando Liquidated Items API
  slug: zalando-liquidated-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-liquidated-items-api-openapi.yml
- filename: zalando-logistic-centers-api-openapi.yml
  format: yaml
  label: Zalando Logistic Centers API
  slug: zalando-logistic-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-logistic-centers-api-openapi.yml
- filename: zalando-offer-blockers-api-openapi.yml
  format: yaml
  label: Zalando offer-blockers API
  slug: zalando-offer-blockers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-offer-blockers-api-openapi.yml
- filename: zalando-orders-api-openapi.yml
  format: yaml
  label: Zalando Orders API
  slug: zalando-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-orders-api-openapi.yml
- filename: zalando-outlines-api-openapi.yml
  format: yaml
  label: Zalando Outlines API
  slug: zalando-outlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-outlines-api-openapi.yml
- filename: zalando-prices-api-openapi.yml
  format: yaml
  label: Zalando prices API
  slug: zalando-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-prices-api-openapi.yml
- filename: zalando-product-association-api-openapi.yml
  format: yaml
  label: Zalando Product Association API
  slug: zalando-product-association-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-product-association-api-openapi.yml
- filename: zalando-reports-api-openapi.yml
  format: yaml
  label: Zalando Reports API
  slug: zalando-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-reports-api-openapi.yml
- filename: zalando-returned-items-api-openapi.yml
  format: yaml
  label: Zalando Returned Items API
  slug: zalando-returned-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-returned-items-api-openapi.yml
- filename: zalando-saleschannels-api-openapi.yml
  format: yaml
  label: Zalando SalesChannels API
  slug: zalando-saleschannels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-saleschannels-api-openapi.yml
- filename: zalando-shipments-api-openapi.yml
  format: yaml
  label: Zalando Shipments API
  slug: zalando-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-shipments-api-openapi.yml
- filename: zalando-stocks-api-openapi.yml
  format: yaml
  label: Zalando stocks API
  slug: zalando-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-stocks-api-openapi.yml
- filename: zalando-types-api-openapi.yml
  format: yaml
  label: Zalando Types API
  slug: zalando-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-types-api-openapi.yml
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
