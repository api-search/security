---
anonymous_access: false
api_key_in: []
api_specs:
- filename: auctiontrace-com-buyer-client-api-openapi.yml
  format: yaml
  label: AuctionTrace Buyer Client API
  slug: auctiontrace-com-buyer-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-buyer-client-api-openapi.yml
- filename: auctiontrace-com-buyer-kit-api-openapi.yml
  format: yaml
  label: AuctionTrace Buyer Kit API
  slug: auctiontrace-com-buyer-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-buyer-kit-api-openapi.yml
- filename: auctiontrace-com-catalog-api-openapi.yml
  format: yaml
  label: AuctionTrace Catalog API
  slug: auctiontrace-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-catalog-api-openapi.yml
- filename: auctiontrace-com-datasets-api-openapi.yml
  format: yaml
  label: AuctionTrace Datasets API
  slug: auctiontrace-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-datasets-api-openapi.yml
- filename: auctiontrace-com-healthz-api-openapi.yml
  format: yaml
  label: AuctionTrace Healthz API
  slug: auctiontrace-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-healthz-api-openapi.yml
- filename: auctiontrace-com-human-checkout-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Checkout API
  slug: auctiontrace-com-human-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-checkout-api-openapi.yml
- filename: auctiontrace-com-human-interest-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Interest API
  slug: auctiontrace-com-human-interest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-interest-api-openapi.yml
- filename: auctiontrace-com-human-offers-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Offers API
  slug: auctiontrace-com-human-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-offers-api-openapi.yml
- filename: auctiontrace-com-human-orders-api-openapi.yml
  format: yaml
  label: AuctionTrace Human Orders API
  slug: auctiontrace-com-human-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-human-orders-api-openapi.yml
- filename: auctiontrace-com-offer-feedback-api-openapi.yml
  format: yaml
  label: AuctionTrace Offer Feedback API
  slug: auctiontrace-com-offer-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-offer-feedback-api-openapi.yml
- filename: auctiontrace-com-outcome-assessment-api-openapi.yml
  format: yaml
  label: AuctionTrace Outcome Assessment API
  slug: auctiontrace-com-outcome-assessment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-outcome-assessment-api-openapi.yml
- filename: auctiontrace-com-trade-list-api-openapi.yml
  format: yaml
  label: AuctionTrace Trade List API
  slug: auctiontrace-com-trade-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auctiontrace-com/openapi/auctiontrace-com-trade-list-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Auctiontrace Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AuctionTrace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AuctionTrace
provider_slug: auctiontrace-com
scheme_count: 1
schemes:
- bearerFormat: opaque-order-access-token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/auctiontrace-com-openapi.json
  type: http
slug: auctiontrace-com-authentication
source_filename: auctiontrace-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/auctiontrace-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque-order-access-token\n  sources:\n  - openapi/auctiontrace-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/auctiontrace-com/authentication/auctiontrace-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Trading
- Analytics
- Finance
- ES-Strategy
---
