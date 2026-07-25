---
api_specs:
- filename: pendle-assets-api-openapi.yml
  format: yaml
  label: Pendle Assets API
  slug: pendle-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-assets-api-openapi.yml
- filename: pendle-chains-api-openapi.yml
  format: yaml
  label: Pendle Chains API
  slug: pendle-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-chains-api-openapi.yml
- filename: pendle-dashboard-api-openapi.yml
  format: yaml
  label: Pendle Dashboard API
  slug: pendle-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-dashboard-api-openapi.yml
- filename: pendle-limit-orders-api-openapi.yml
  format: yaml
  label: Pendle Limit Orders API
  slug: pendle-limit-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-limit-orders-api-openapi.yml
- filename: pendle-markets-api-openapi.yml
  format: yaml
  label: Pendle Markets API
  slug: pendle-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-markets-api-openapi.yml
- filename: pendle-pendle-emission-api-openapi.yml
  format: yaml
  label: Pendle Pendle Emission API
  slug: pendle-pendle-emission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-pendle-emission-api-openapi.yml
- filename: pendle-sdk-api-openapi.yml
  format: yaml
  label: Pendle SDK API
  slug: pendle-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-sdk-api-openapi.yml
- filename: pendle-statistics-api-openapi.yml
  format: yaml
  label: Pendle Statistics API
  slug: pendle-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-statistics-api-openapi.yml
- filename: pendle-transactions-api-openapi.yml
  format: yaml
  label: Pendle Transactions API
  slug: pendle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-transactions-api-openapi.yml
- filename: pendle-ve-pendle-api-openapi.yml
  format: yaml
  label: Pendle Ve Pendle API
  slug: pendle-ve-pendle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/openapi/pendle-ve-pendle-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pendle.finance
  spf: true
hosts:
- cert_expires: Aug 20 15:58:09 2026 GMT
  host: www.pendle.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 13:02:18 2026 GMT
  host: docs.pendle.finance
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 15:58:09 2026 GMT
  host: api-v2.pendle.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pendle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pendle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pendle
provider_slug: pendle
slug: pendle-domain-security
source_filename: pendle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pendle.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:58:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pendle.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:02:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api-v2.pendle.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:58:09 2026 GMT\n  hsts: null\ndomains:\n- domain: pendle.finance\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/security/pendle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- DeFi
- Yield Tokenization
- Crypto
- Principal Tokens
- Yield Tokens
- AMM
- Liquidity Pools
---
