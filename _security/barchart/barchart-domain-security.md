---
api_specs:
- filename: barchart-charts-and-analytics-api-openapi.yml
  format: yaml
  label: Barchart Charts and Analytics API
  slug: barchart-charts-and-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-charts-and-analytics-api-openapi.yml
- filename: barchart-cryptocurrency-data-api-openapi.yml
  format: yaml
  label: Barchart Cryptocurrency Data API
  slug: barchart-cryptocurrency-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-cryptocurrency-data-api-openapi.yml
- filename: barchart-leaderboards-and-lists-api-openapi.yml
  format: yaml
  label: Barchart Leaderboards and Lists API
  slug: barchart-leaderboards-and-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-leaderboards-and-lists-api-openapi.yml
- filename: barchart-metadata-api-openapi.yml
  format: yaml
  label: Barchart Metadata API
  slug: barchart-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-metadata-api-openapi.yml
- filename: barchart-news-and-filings-api-openapi.yml
  format: yaml
  label: Barchart News and Filings API
  slug: barchart-news-and-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-news-and-filings-api-openapi.yml
- filename: barchart-other-data-api-openapi.yml
  format: yaml
  label: Barchart Other Data API
  slug: barchart-other-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-other-data-api-openapi.yml
- filename: barchart-price-data-api-openapi.yml
  format: yaml
  label: Barchart Price Data API
  slug: barchart-price-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-price-data-api-openapi.yml
- filename: barchart-profiles-and-financial-data-api-openapi.yml
  format: yaml
  label: Barchart Profiles and Financial Data API
  slug: barchart-profiles-and-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-profiles-and-financial-data-api-openapi.yml
- filename: barchart-splits-dividends-and-earnings-api-openapi.yml
  format: yaml
  label: Barchart Splits, Dividends, and Earnings API
  slug: barchart-splits-dividends-and-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-splits-dividends-and-earnings-api-openapi.yml
- filename: barchart-etfs-api-openapi.yml
  format: yaml
  label: Barchart ET Fs API
  slug: barchart-etfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-etfs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:caa-notify@barchart.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: barchart.com
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.barchart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: ondemand.websol.barchart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Barchart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barchart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barchart
provider_slug: barchart
slug: barchart-domain-security
source_filename: barchart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barchart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ondemand.websol.barchart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: barchart.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:caa-notify@barchart.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/security/barchart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Market Data
- Financial Data
- Commodities
- Futures
- Options
- Reference Data
- Stocks
- Historical Data
- Cryptocurrency
- Agriculture
---
