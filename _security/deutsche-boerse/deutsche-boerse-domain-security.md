---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deutsche-boerse.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.deutsche-boerse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: console.developer.deutsche-boerse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 23:59:59 2026 GMT
  host: a7.deutsche-boerse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deutsche Boerse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deutsche Börse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deutsche Börse
provider_slug: deutsche-boerse
slug: deutsche-boerse-domain-security
source_filename: deutsche-boerse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deutsche-boerse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.developer.deutsche-boerse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: a7.deutsche-boerse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deutsche-boerse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-boerse/refs/heads/main/security/deutsche-boerse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
