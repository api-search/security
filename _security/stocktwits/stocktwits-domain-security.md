---
api_specs:
- filename: stocktwits-account-api-openapi.yml
  format: yaml
  label: StockTwits Account API
  slug: stocktwits-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-account-api-openapi.yml
- filename: stocktwits-deletions-api-openapi.yml
  format: yaml
  label: StockTwits Deletions API
  slug: stocktwits-deletions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-deletions-api-openapi.yml
- filename: stocktwits-friendships-api-openapi.yml
  format: yaml
  label: StockTwits Friendships API
  slug: stocktwits-friendships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-friendships-api-openapi.yml
- filename: stocktwits-graph-social-api-openapi.yml
  format: yaml
  label: StockTwits Graph (Social) API
  slug: stocktwits-graph-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-graph-social-api-openapi.yml
- filename: stocktwits-messages-api-openapi.yml
  format: yaml
  label: StockTwits Messages API
  slug: stocktwits-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-messages-api-openapi.yml
- filename: stocktwits-search-api-openapi.yml
  format: yaml
  label: StockTwits Search API
  slug: stocktwits-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-search-api-openapi.yml
- filename: stocktwits-streams-api-openapi.yml
  format: yaml
  label: StockTwits Streams API
  slug: stocktwits-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-streams-api-openapi.yml
- filename: stocktwits-trending-api-openapi.yml
  format: yaml
  label: StockTwits Trending API
  slug: stocktwits-trending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-trending-api-openapi.yml
- filename: stocktwits-watchlists-api-openapi.yml
  format: yaml
  label: StockTwits Watchlists API
  slug: stocktwits-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-watchlists-api-openapi.yml
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
