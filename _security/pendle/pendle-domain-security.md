---
api_specs:
- filename: open-api.json
  format: json
  label: Pendle V2 Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/pendle-finance/documentation/master/static/pendle-dev-docs/openapi/open-api.json
- filename: open-api.json
  format: json
  label: Pendle Hosted SDK
  slug: hosted-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/pendle-finance/documentation/master/static/pendle-dev-docs/openapi/open-api.json
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
