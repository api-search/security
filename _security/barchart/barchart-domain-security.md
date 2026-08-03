---
api_specs:
- filename: barchart-commodities-agriculture-api-openapi.yml
  format: yaml
  label: Barchart Commodities & Agriculture API
  slug: barchart-commodities-agriculture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-commodities-agriculture-api-openapi.yml
- filename: barchart-corporate-actions-earnings-api-openapi.yml
  format: yaml
  label: Barchart Corporate Actions & Earnings API
  slug: barchart-corporate-actions-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-corporate-actions-earnings-api-openapi.yml
- filename: barchart-cryptocurrency-api-openapi.yml
  format: yaml
  label: Barchart Cryptocurrency API
  slug: barchart-cryptocurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-cryptocurrency-api-openapi.yml
- filename: barchart-fundamentals-api-openapi.yml
  format: yaml
  label: Barchart Fundamentals API
  slug: barchart-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-fundamentals-api-openapi.yml
- filename: barchart-futures-options-api-openapi.yml
  format: yaml
  label: Barchart Futures & Options API
  slug: barchart-futures-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-futures-options-api-openapi.yml
- filename: barchart-history-api-openapi.yml
  format: yaml
  label: Barchart History API
  slug: barchart-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-history-api-openapi.yml
- filename: barchart-news-filings-api-openapi.yml
  format: yaml
  label: Barchart News & Filings API
  slug: barchart-news-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-news-filings-api-openapi.yml
- filename: barchart-quotes-api-openapi.yml
  format: yaml
  label: Barchart Quotes API
  slug: barchart-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-quotes-api-openapi.yml
- filename: barchart-reference-equities-api-openapi.yml
  format: yaml
  label: Barchart Reference & Equities API
  slug: barchart-reference-equities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-reference-equities-api-openapi.yml
- filename: barchart-technicals-charts-api-openapi.yml
  format: yaml
  label: Barchart Technicals & Charts API
  slug: barchart-technicals-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-technicals-charts-api-openapi.yml
- filename: barchart-weather-api-openapi.yml
  format: yaml
  label: Barchart Weather API
  slug: barchart-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-weather-api-openapi.yml
- filename: barchart-ondemand-official-openapi.yml
  format: yaml
  label: Barchart OnDemand APIs
  slug: barchart-ondemand-official-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-ondemand-official-openapi.yml
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
- Equities
- Historical Data
- Cryptocurrency
- Agriculture
---
