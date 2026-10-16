---
api_specs:
- filename: btcmarkets-account-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Account APIs API
  slug: btcmarkets-account-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-account-apis-api-openapi.yml
- filename: btcmarkets-batch-order-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Batch Order APIs API
  slug: btcmarkets-batch-order-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-batch-order-apis-api-openapi.yml
- filename: btcmarkets-fund-management-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Fund Management APIs API
  slug: btcmarkets-fund-management-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-fund-management-apis-api-openapi.yml
- filename: btcmarkets-market-data-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Market Data APIs API
  slug: btcmarkets-market-data-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-market-data-apis-api-openapi.yml
- filename: btcmarkets-misc-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Misc APIs API
  slug: btcmarkets-misc-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-misc-apis-api-openapi.yml
- filename: btcmarkets-order-placement-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Order Placement APIs API
  slug: btcmarkets-order-placement-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-order-placement-apis-api-openapi.yml
- filename: btcmarkets-report-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Report APIs API
  slug: btcmarkets-report-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-report-apis-api-openapi.yml
- filename: btcmarkets-trade-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Trade APIs API
  slug: btcmarkets-trade-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-trade-apis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: btcmarkets.net
  spf: true
hosts:
- cert_expires: Nov 25 22:20:42 2026 GMT
  host: www.btcmarkets.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Btcmarkets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BTC Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BTC Markets
provider_slug: btcmarkets
slug: btcmarkets-domain-security
source_filename: btcmarkets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.btcmarkets.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: btcmarkets.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/security/btcmarkets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Australia
---
