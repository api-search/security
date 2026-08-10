---
api_specs:
- filename: caplight-companies-api-openapi.yml
  format: yaml
  label: Caplight Companies API
  slug: caplight-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-companies-api-openapi.yml
- filename: caplight-company-api-openapi.yml
  format: yaml
  label: Caplight Company API
  slug: caplight-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-api-openapi.yml
- filename: caplight-company-details-api-openapi.yml
  format: yaml
  label: Caplight Company Details API
  slug: caplight-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-details-api-openapi.yml
- filename: caplight-company-filings-api-openapi.yml
  format: yaml
  label: Caplight Company Filings API
  slug: caplight-company-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-filings-api-openapi.yml
- filename: caplight-company-lookup-api-openapi.yml
  format: yaml
  label: Caplight Company Lookup API
  slug: caplight-company-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-lookup-api-openapi.yml
- filename: caplight-composite-index-api-openapi.yml
  format: yaml
  label: Caplight Composite Index API
  slug: caplight-composite-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-composite-index-api-openapi.yml
- filename: caplight-comps-api-openapi.yml
  format: yaml
  label: Caplight Comps API
  slug: caplight-comps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-comps-api-openapi.yml
- filename: caplight-fund-marks-api-openapi.yml
  format: yaml
  label: Caplight Fund Marks API
  slug: caplight-fund-marks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-fund-marks-api-openapi.yml
- filename: caplight-funding-rounds-api-openapi.yml
  format: yaml
  label: Caplight Funding Rounds API
  slug: caplight-funding-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-funding-rounds-api-openapi.yml
- filename: caplight-investors-api-openapi.yml
  format: yaml
  label: Caplight Investors API
  slug: caplight-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-investors-api-openapi.yml
- filename: caplight-live-orderbook-api-openapi.yml
  format: yaml
  label: Caplight Live Orderbook API
  slug: caplight-live-orderbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-live-orderbook-api-openapi.yml
- filename: caplight-marketprice-api-openapi.yml
  format: yaml
  label: Caplight Market Price API
  slug: caplight-marketprice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-marketprice-api-openapi.yml
- filename: caplight-news-api-openapi.yml
  format: yaml
  label: Caplight News API
  slug: caplight-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-news-api-openapi.yml
- filename: caplight-order-history-api-openapi.yml
  format: yaml
  label: Caplight Order History API
  slug: caplight-order-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-order-history-api-openapi.yml
- filename: caplight-stock-splits-api-openapi.yml
  format: yaml
  label: Caplight Stock Splits API
  slug: caplight-stock-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-stock-splits-api-openapi.yml
- filename: caplight-trade-history-api-openapi.yml
  format: yaml
  label: Caplight Trade History API
  slug: caplight-trade-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-trade-history-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: caplight.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudfunctions.net
  spf: true
hosts:
- cert_expires: Sep 25 06:48:59 2026 GMT
  host: www.caplight.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:25:00 2026 GMT
  host: platform.caplight.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:06:28 2026 GMT
  host: us-central1-caplight-prod.cloudfunctions.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caplight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caplight, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Caplight
provider_slug: caplight
slug: caplight-domain-security
source_filename: caplight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caplight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:48:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.caplight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:25:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: us-central1-caplight-prod.cloudfunctions.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:06:28 2026 GMT\n  hsts: null\ndomains:\n- domain: caplight.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cloudfunctions.net\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/security/caplight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- private-markets
- secondary-market
- market-data
- venture-capital
- company-data
- investor-data
- funding-rounds
- pricing-data
- financial-data
- fintech
- mcp
- agent-native
---
