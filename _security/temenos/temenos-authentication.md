---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Temenos Transact API
  slug: temenos-transact-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/transact/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Infinity API
  slug: temenos-infinity-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/infinity/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Payments API
  slug: temenos-payments-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/payments/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Fund Administration API
  slug: temenos-fund-administration-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/funds/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Financial Crime Mitigation API
  slug: temenos-financial-crime-mitigation-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/fcm/openapi.json
- filename: temenos-data-hub-openapi.yml
  format: yaml
  label: Temenos Transact Data Hub API
  slug: temenos-transact-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-data-hub-openapi.yml
- filename: temenos-wealth-openapi.yml
  format: yaml
  label: Temenos Wealth API
  slug: temenos-wealth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-wealth-openapi.yml
- filename: temenos-enterprise-product-pricing-openapi.yml
  format: yaml
  label: Temenos Enterprise Product and Pricing API
  slug: temenos-enterprise-product-and-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-enterprise-product-pricing-openapi.yml
- filename: temenos-cloud-banking-openapi.yml
  format: yaml
  label: Temenos Cloud Banking (CMB) API
  slug: temenos-cloud-banking-cmb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-cloud-banking-openapi.yml
- filename: temenos-journey-manager-openapi.yml
  format: yaml
  label: Temenos Journey Manager API
  slug: temenos-journey-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-journey-manager-openapi.yml
- filename: temenos-microservices-openapi.yml
  format: yaml
  label: Temenos Transact Microservices API
  slug: temenos-transact-microservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-microservices-openapi.yml
- filename: temenos-bnpl-openapi.yml
  format: yaml
  label: Temenos Buy Now Pay Later API
  slug: temenos-buy-now-pay-later-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-bnpl-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Temenos Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Temenos secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Temenos
provider_slug: temenos
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/temenos-bnpl-openapi.yml
  - openapi/temenos-cloud-banking-openapi.yml
  - openapi/temenos-data-hub-openapi.yml
  - openapi/temenos-enterprise-product-pricing-openapi.yml
  - openapi/temenos-financial-crime-mitigation-openapi.yml
  - openapi/temenos-fund-administration-openapi.yml
  - openapi/temenos-infinity-openapi.yml
  - openapi/temenos-journey-manager-openapi.yml
  - openapi/temenos-microservices-openapi.yml
  - openapi/temenos-payments-openapi.yml
  - openapi/temenos-transact-openapi.yml
  - openapi/temenos-wealth-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://journey.temenos.com/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://journey.temenos.com/oauth2/token
  name: oauth2
  sources:
  - openapi/temenos-journey-manager-openapi.yml
  - openapi/temenos-transact-openapi.yml
  type: oauth2
slug: temenos-authentication
source_filename: temenos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temenos-bnpl-openapi.yml, openapi/temenos-cloud-banking-openapi.yml, openapi/temenos-data-hub-openapi.yml,\n  openapi/temenos-enterprise-product-pricing-openapi.yml, openapi/temenos-financial-crime-mitigation-openapi.yml,\n  openapi/temenos-fund-administration-openapi.yml, openapi/temenos-infinity-openapi.yml, openapi/temenos-journey-manager-openapi.yml,\n  openapi/temenos-microservices-openapi.yml, openapi/temenos-payments-openapi.yml, openapi/temenos-transact-openapi.yml,\n  openapi/temenos-wealth-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/temenos-bnpl-openapi.yml\n  - openapi/temenos-cloud-banking-openapi.yml\n  - openapi/temenos-data-hub-openapi.yml\n  - openapi/temenos-enterprise-product-pricing-openapi.yml\n  - openapi/temenos-financial-crime-mitigation-openapi.yml\n\
  \  - openapi/temenos-fund-administration-openapi.yml\n  - openapi/temenos-infinity-openapi.yml\n  - openapi/temenos-journey-manager-openapi.yml\n  - openapi/temenos-microservices-openapi.yml\n  - openapi/temenos-payments-openapi.yml\n  - openapi/temenos-transact-openapi.yml\n  - openapi/temenos-wealth-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://journey.temenos.com/oauth2/authorize\n    tokenUrl: https://journey.temenos.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/temenos-journey-manager-openapi.yml\n  - openapi/temenos-transact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/authentication/temenos-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
---
