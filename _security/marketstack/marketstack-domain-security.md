---
api_specs:
- filename: marketstack-bonds-api-openapi.yml
  format: yaml
  label: Marketstack Bonds API
  slug: marketstack-bonds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-bonds-api-openapi.yml
- filename: marketstack-commodities-api-openapi.yml
  format: yaml
  label: Marketstack Commodities API
  slug: marketstack-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-commodities-api-openapi.yml
- filename: marketstack-company-ratings-api-openapi.yml
  format: yaml
  label: Marketstack Company Ratings API
  slug: marketstack-company-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-company-ratings-api-openapi.yml
- filename: marketstack-currencies-api-openapi.yml
  format: yaml
  label: Marketstack Currencies API
  slug: marketstack-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-currencies-api-openapi.yml
- filename: marketstack-dividends-api-openapi.yml
  format: yaml
  label: Marketstack Dividends API
  slug: marketstack-dividends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-dividends-api-openapi.yml
- filename: marketstack-edgar-api-openapi.yml
  format: yaml
  label: Marketstack EDGAR API
  slug: marketstack-edgar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-edgar-api-openapi.yml
- filename: marketstack-end-of-day-api-openapi.yml
  format: yaml
  label: Marketstack End Of Day API
  slug: marketstack-end-of-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-end-of-day-api-openapi.yml
- filename: marketstack-etfs-api-openapi.yml
  format: yaml
  label: Marketstack ET Fs API
  slug: marketstack-etfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-etfs-api-openapi.yml
- filename: marketstack-exchanges-api-openapi.yml
  format: yaml
  label: Marketstack Exchanges API
  slug: marketstack-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-exchanges-api-openapi.yml
- filename: marketstack-indexes-api-openapi.yml
  format: yaml
  label: Marketstack Indexes API
  slug: marketstack-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-indexes-api-openapi.yml
- filename: marketstack-intraday-api-openapi.yml
  format: yaml
  label: Marketstack Intraday API
  slug: marketstack-intraday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-intraday-api-openapi.yml
- filename: marketstack-splits-api-openapi.yml
  format: yaml
  label: Marketstack Splits API
  slug: marketstack-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-splits-api-openapi.yml
- filename: marketstack-stock-prices-api-openapi.yml
  format: yaml
  label: Marketstack Stock Prices API
  slug: marketstack-stock-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-stock-prices-api-openapi.yml
- filename: marketstack-tickers-api-openapi.yml
  format: yaml
  label: Marketstack Tickers API
  slug: marketstack-tickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-tickers-api-openapi.yml
- filename: marketstack-timezones-api-openapi.yml
  format: yaml
  label: Marketstack Timezones API
  slug: marketstack-timezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-timezones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketstack.com
  spf: true
hosts:
- cert_expires: Aug 27 22:59:05 2026 GMT
  host: marketstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 22:59:05 2026 GMT
  host: api.marketstack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marketstack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marketstack
provider_slug: marketstack
slug: marketstack-domain-security
source_filename: marketstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:59:05 2026 GMT\n  hsts: false\n- host: api.marketstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:59:05 2026 GMT\n  hsts: null\ndomains:\n- domain: marketstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/security/marketstack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Stock Market
- Market Data
- End-of-Day Data
- Intraday Data
- Commodities
- Bonds
- ETFs
- SEC EDGAR
- Dividends
---
