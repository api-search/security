---
api_specs:
- filename: stockx-public-openapi-original.json
  format: json
  label: StockX Public API
  slug: stockx-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-public-openapi-original.json
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
- Orders
---
