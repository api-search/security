---
api_key_in:
- header
api_specs:
- filename: deutsche-boerse-order-book-api-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Order Book API
  slug: a7-order-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-order-book-api-api-openapi.yml
- filename: deutsche-boerse-market-data-api-eobi-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Market Data API (EOBI)
  slug: a7-market-data-eobi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-market-data-api-eobi-api-openapi.yml
- filename: deutsche-boerse-exchanges-assets-securities-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - CME Market Data API (MDP)
  slug: a7-cme-market-data-mdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-exchanges-assets-securities-api-openapi.yml
- filename: deutsche-boerse-reference-data-api-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Reference Data API (RDI) v2
  slug: a7-reference-data-rdi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-reference-data-api-api-openapi.yml
- filename: deutsche-boerse-cme-reference-data-api-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - CME Reference Data API (SD)
  slug: a7-cme-reference-data-sd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-cme-reference-data-api-api-openapi.yml
- filename: deutsche-boerse-algo-management-api-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Algo Management API
  slug: a7-algo-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-algo-management-api-api-openapi.yml
- filename: deutsche-boerse-dataset-api-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Dataset API
  slug: a7-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-dataset-api-api-openapi.yml
- filename: deutsche-boerse-latency-historgram-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Market Data Insights API
  slug: a7-market-data-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-latency-historgram-api-openapi.yml
- filename: deutsche-boerse-option-prices-and-greeks-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Option Analytics API
  slug: a7-option-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-option-prices-and-greeks-api-openapi.yml
- filename: deutsche-boerse-precalc-api-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Precalc API
  slug: a7-precalc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-precalc-api-api-openapi.yml
- filename: deutsche-boerse-auctions-api-openapi.yml
  format: yaml
  label: A7 Analytics Platform - Auction Simulation API
  slug: a7-auction-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/openapi/deutsche-boerse-auctions-api-openapi.yml
- filename: deutsche-boerse-cloud-stream-asyncapi.yml
  format: yaml
  label: Deutsche Börse Cloud Stream Market Data API
  slug: cloud-stream-market-data-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/asyncapi/deutsche-boerse-cloud-stream-asyncapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Deutsche Boerse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deutsche Börse secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Deutsche Börse
provider_slug: deutsche-boerse
scheme_count: 3
schemes:
- docs: https://docs.developer.deutsche-boerse.com/docs/consumer/getting-started/consume/
  in: header
  name: X-DBP-APIKEY
  parameter: X-DBP-APIKEY
  sources:
  - https://docs.developer.deutsche-boerse.com/docs/consumer/getting-started/consume/
  - https://www.eurex.com/ex-en/data/free-reference-data-api
  type: apiKey
- docs: https://docs.developer.deutsche-boerse.com/docs/consumer/mTLS-consumer
  name: mutualTLS (per-API option)
  sources:
  - https://docs.developer.deutsche-boerse.com/docs/consumer/mTLS-consumer
  type: mutualTLS
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/deutsche-boerse-algo-management-api-api-openapi.yml
  - openapi/deutsche-boerse-auctions-api-openapi.yml
  - openapi/deutsche-boerse-cme-reference-data-api-api-openapi.yml
  - openapi/deutsche-boerse-dataset-api-api-openapi.yml
  - openapi/deutsche-boerse-datasets-api-openapi.yml
  - openapi/deutsche-boerse-exchanges-assets-securities-api-openapi.yml
  - openapi/deutsche-boerse-exchanges-symbols-securities-api-openapi.yml
  - openapi/deutsche-boerse-historical-time-series-api-openapi.yml
  - openapi/deutsche-boerse-indicators-api-openapi.yml
  - openapi/deutsche-boerse-latency-historgram-api-openapi.yml
  - openapi/deutsche-boerse-market-data-api-eobi-api-openapi.yml
  - openapi/deutsche-boerse-option-prices-and-greeks-api-openapi.yml
  - openapi/deutsche-boerse-order-book-api-api-openapi.yml
  - openapi/deutsche-boerse-pace-of-the-roll-api-openapi.yml
  - openapi/deutsche-boerse-precalc-api-api-openapi.yml
  - openapi/deutsche-boerse-reference-data-api-api-openapi.yml
  - openapi/deutsche-boerse-sending-times-packets-messages-api-openapi.yml
  - openapi/deutsche-boerse-symbols-api-openapi.yml
  type: http
slug: deutsche-boerse-authentication
source_filename: deutsche-boerse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://docs.developer.deutsche-boerse.com/docs/consumer/getting-started/consume/\nsource: openapi/deutsche-boerse-algo-management-api-api-openapi.yml, openapi/deutsche-boerse-auctions-api-openapi.yml,\n  openapi/deutsche-boerse-cme-reference-data-api-api-openapi.yml, openapi/deutsche-boerse-dataset-api-api-openapi.yml,\n  openapi/deutsche-boerse-datasets-api-openapi.yml, openapi/deutsche-boerse-exchanges-assets-securities-api-openapi.yml,\n  openapi/deutsche-boerse-exchanges-symbols-securities-api-openapi.yml, openapi/deutsche-boerse-historical-time-series-api-openapi.yml,\n  openapi/deutsche-boerse-indicators-api-openapi.yml, openapi/deutsche-boerse-latency-historgram-api-openapi.yml,\n  openapi/deutsche-boerse-market-data-api-eobi-api-openapi.yml, openapi/deutsche-boerse-option-prices-and-greeks-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  notes: A7 Analytics Platform APIs\
  \ use HTTP Bearer tokens issued in the A7 GUI\n    (derived from all 18 OpenAPI specs). Group API Platform APIs use an API key in\n    the X-DBP-APIKEY header, generated per application in the developer console;\n    some publishers additionally require mutual TLS (X.509 client certificates) or\n    publisher-issued keys. OAuth2/OIDC is documented as \"Coming soon\". The free\n    Eurex T7 reference data GraphQL API accepts a published shared rate-limited\n    X-DBP-APIKEY (see https://www.eurex.com/ex-en/data/free-reference-data-api).\nschemes:\n- name: X-DBP-APIKEY\n  type: apiKey\n  in: header\n  parameter: X-DBP-APIKEY\n  docs: https://docs.developer.deutsche-boerse.com/docs/consumer/getting-started/consume/\n  sources:\n  - https://docs.developer.deutsche-boerse.com/docs/consumer/getting-started/consume/\n  - https://www.eurex.com/ex-en/data/free-reference-data-api\n- name: mutualTLS (per-API option)\n  type: mutualTLS\n  docs: https://docs.developer.deutsche-boerse.com/docs/consumer/mTLS-consumer\n\
  \  sources:\n  - https://docs.developer.deutsche-boerse.com/docs/consumer/mTLS-consumer\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/deutsche-boerse-algo-management-api-api-openapi.yml\n  - openapi/deutsche-boerse-auctions-api-openapi.yml\n  - openapi/deutsche-boerse-cme-reference-data-api-api-openapi.yml\n  - openapi/deutsche-boerse-dataset-api-api-openapi.yml\n  - openapi/deutsche-boerse-datasets-api-openapi.yml\n  - openapi/deutsche-boerse-exchanges-assets-securities-api-openapi.yml\n  - openapi/deutsche-boerse-exchanges-symbols-securities-api-openapi.yml\n  - openapi/deutsche-boerse-historical-time-series-api-openapi.yml\n  - openapi/deutsche-boerse-indicators-api-openapi.yml\n  - openapi/deutsche-boerse-latency-historgram-api-openapi.yml\n  - openapi/deutsche-boerse-market-data-api-eobi-api-openapi.yml\n  - openapi/deutsche-boerse-option-prices-and-greeks-api-openapi.yml\n  - openapi/deutsche-boerse-order-book-api-api-openapi.yml\n  - openapi/deutsche-boerse-pace-of-the-roll-api-openapi.yml\n\
  \  - openapi/deutsche-boerse-precalc-api-api-openapi.yml\n  - openapi/deutsche-boerse-reference-data-api-api-openapi.yml\n  - openapi/deutsche-boerse-sending-times-packets-messages-api-openapi.yml\n  - openapi/deutsche-boerse-symbols-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/authentication/deutsche-boerse-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Financial
- Market Data
- Stocks
- Derivatives
- Trading
- Real-Time
- Order Book
- Reference Data
- Exchange
- Analytics
---
