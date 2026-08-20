---
api_specs:
- filename: stockx-batch-api-openapi.yml
  format: yaml
  label: StockX Batch API
  slug: stockx-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-batch-api-openapi.yml
- filename: stockx-catalog-api-openapi.yml
  format: yaml
  label: StockX Catalog API
  slug: stockx-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-catalog-api-openapi.yml
- filename: stockx-listings-api-openapi.yml
  format: yaml
  label: StockX Listings API
  slug: stockx-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-listings-api-openapi.yml
- filename: stockx-order-api-openapi.yml
  format: yaml
  label: StockX Order API
  slug: stockx-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-order-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stockx.com
  spf: true
hosts:
- cert_expires: Oct 12 04:03:34 2026 GMT
  host: stockx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:03:34 2026 GMT
  host: api.stockx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stockx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StockX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StockX
provider_slug: stockx
slug: stockx-domain-security
source_filename: stockx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stockx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:03:34 2026 GMT\n  hsts: null\n- host: api.stockx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:03:34 2026 GMT\n  hsts: null\ndomains:\n- domain: stockx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/security/stockx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- E-Commerce
- Sneakers
- Streetwear
- Resale
- Collectibles
- Catalog
- Selling
- Order
---
