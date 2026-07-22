---
api_specs:
- filename: ondo-finance-gm-openapi-original.json
  format: json
  label: Ondo GM Backend API (Ondo Stocks / Global Markets)
  slug: ondo-gm-backend-api-ondo-stocks-global-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/openapi/ondo-finance-gm-openapi-original.json
- filename: ondo-finance-perps-openapi-original.json
  format: json
  label: Ondo Perps REST API
  slug: ondo-perps-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/openapi/ondo-finance-perps-openapi-original.json
- filename: ondo-finance-perps-ws-openapi-original.json
  format: json
  label: Ondo Perps WebSocket API
  slug: ondo-perps-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/openapi/ondo-finance-perps-ws-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ondo.finance
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ondoperps.xyz
  spf: true
hosts:
- cert_expires: Aug 21 05:09:08 2026 GMT
  host: ondo.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.gm.ondo.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:06:55 2026 GMT
  host: api.ondoperps.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ondo Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ondo Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ondo Finance
provider_slug: ondo-finance
slug: ondo-finance-domain-security
source_filename: ondo-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ondo.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 05:09:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gm.ondo.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.ondoperps.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:06:55 2026 GMT\n  hsts: null\ndomains:\n- domain: ondo.finance\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ondoperps.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/security/ondo-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Tokenization
- Real World Assets
- DeFi
- Stocks
- Trading
- Perpetual Futures
- Market Data
- Blockchain
- Financial Services
---
