---
api_specs:
- filename: stocktwits-openapi-original.json
  format: json
  label: StockTwits API v2
  slug: stocktwits-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stocktwits.com
  spf: true
hosts:
- cert_expires: Sep 13 08:58:59 2026 GMT
  host: stocktwits.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:58:59 2026 GMT
  host: api.stocktwits.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stocktwits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StockTwits, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StockTwits
provider_slug: stocktwits
slug: stocktwits-domain-security
source_filename: stocktwits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stocktwits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:58:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.stocktwits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:58:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stocktwits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/security/stocktwits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Social
- Stocks
- Trading
- Investing
- Market Data
- Social Finance
- Watchlists
- Messaging
---
