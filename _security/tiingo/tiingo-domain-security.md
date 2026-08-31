---
api_specs:
- filename: tiingo-boats-api-openapi.yml
  format: yaml
  label: Tiingo BOATS API
  slug: tiingo-boats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-boats-api-openapi.yml
- filename: tiingo-corporate-actions-api-openapi.yml
  format: yaml
  label: Tiingo Corporate Actions API
  slug: tiingo-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-corporate-actions-api-openapi.yml
- filename: tiingo-crypto-api-openapi.yml
  format: yaml
  label: Tiingo Crypto API
  slug: tiingo-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-crypto-api-openapi.yml
- filename: tiingo-crypto-yield-api-openapi.yml
  format: yaml
  label: Tiingo Crypto Yield API
  slug: tiingo-crypto-yield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-crypto-yield-api-openapi.yml
- filename: tiingo-end-of-day-api-openapi.yml
  format: yaml
  label: Tiingo End Of Day API
  slug: tiingo-end-of-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-end-of-day-api-openapi.yml
- filename: tiingo-equity-realtime-api-openapi.yml
  format: yaml
  label: Tiingo Equity Realtime API
  slug: tiingo-equity-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-equity-realtime-api-openapi.yml
- filename: tiingo-forex-api-openapi.yml
  format: yaml
  label: Tiingo Forex API
  slug: tiingo-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-forex-api-openapi.yml
- filename: tiingo-fund-fees-api-openapi.yml
  format: yaml
  label: Tiingo Fund Fees API
  slug: tiingo-fund-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-fund-fees-api-openapi.yml
- filename: tiingo-fundamentals-api-openapi.yml
  format: yaml
  label: Tiingo Fundamentals API
  slug: tiingo-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-fundamentals-api-openapi.yml
- filename: tiingo-iex-api-openapi.yml
  format: yaml
  label: Tiingo IEX API
  slug: tiingo-iex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-iex-api-openapi.yml
- filename: tiingo-news-api-openapi.yml
  format: yaml
  label: Tiingo News API
  slug: tiingo-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-news-api-openapi.yml
- filename: tiingo-small-exchange-api-openapi.yml
  format: yaml
  label: Tiingo Small Exchange API
  slug: tiingo-small-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-small-exchange-api-openapi.yml
- filename: tiingo-utilities-api-openapi.yml
  format: yaml
  label: Tiingo Utilities API
  slug: tiingo-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tiingo.com
  spf: true
hosts:
- cert_expires: Sep 24 02:59:33 2026 GMT
  host: www.tiingo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:21:41 2026 GMT
  host: api.tiingo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiingo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiingo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tiingo
provider_slug: tiingo
slug: tiingo-domain-security
source_filename: tiingo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:59:33 2026 GMT\n  hsts: false\n- host: api.tiingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:21:41 2026 GMT\n  hsts: false\ndomains:\n- domain: tiingo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/security/tiingo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fintech
- Market Data
- Stocks
- Crypto
- FX
- News
- Fundamentals
- WebSockets
---
