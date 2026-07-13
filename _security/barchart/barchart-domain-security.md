---
api_specs:
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Quotes API
  slug: barchart-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart History API
  slug: barchart-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Reference & Equities API
  slug: barchart-reference-equities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Futures & Options API
  slug: barchart-futures-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Fundamentals API
  slug: barchart-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Corporate Actions & Earnings API
  slug: barchart-corporate-actions-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Cryptocurrency API
  slug: barchart-cryptocurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Commodities & Agriculture API
  slug: barchart-commodities-agriculture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Technicals & Charts API
  slug: barchart-technicals-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart News & Filings API
  slug: barchart-news-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Weather API
  slug: barchart-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_policy: reject
  domain: barchart.com
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.barchart.com
  https: true
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: ondemand.websol.barchart.com
  https: true
kind: domain-security
layout: security
method: probed
name: Barchart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barchart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barchart
provider_slug: barchart
slug: barchart-domain-security
source_filename: barchart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barchart.com\n  https: true\n  cert_expires: Dec 28 23:59:59 2026 GMT\n- host: ondemand.websol.barchart.com\n  https: true\n  cert_expires: Nov  6 23:59:59 2026 GMT\ndomains:\n- domain: barchart.com\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/security/barchart-domain-security.yml
summary_line: DMARC
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
