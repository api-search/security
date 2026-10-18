---
api_specs:
- filename: zebpay-futures-api-openapi.yml
  format: yaml
  label: ZebPay Futures API
  slug: zebpay-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-api-openapi.yml
- filename: zebpay-futures-exchange-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Exchange API
  slug: zebpay-futures-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-exchange-api-openapi.yml
- filename: zebpay-futures-market-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Market API
  slug: zebpay-futures-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-market-api-openapi.yml
- filename: zebpay-futures-trade-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Trade API
  slug: zebpay-futures-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-trade-api-openapi.yml
- filename: zebpay-futures-user-leverage-api-openapi.yml
  format: yaml
  label: ZebPay Futures > User Leverage API
  slug: zebpay-futures-user-leverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-user-leverage-api-openapi.yml
- filename: zebpay-futures-wallet-api-openapi.yml
  format: yaml
  label: ZebPay Futures > Wallet API
  slug: zebpay-futures-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-futures-wallet-api-openapi.yml
- filename: zebpay-market-api-openapi.yml
  format: yaml
  label: ZebPay Market API
  slug: zebpay-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-market-api-openapi.yml
- filename: zebpay-trade-api-api-openapi.yml
  format: yaml
  label: ZebPay Trade API
  slug: zebpay-trade-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/openapi/zebpay-trade-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zebpay.com
  spf: true
hosts:
- cert_expires: Jan  8 07:51:28 2027 GMT
  host: zebpay.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zebpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZebPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ZebPay
provider_slug: zebpay
slug: zebpay-domain-security
source_filename: zebpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zebpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 07:51:28 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: zebpay.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zebpay/refs/heads/main/security/zebpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Futures
- India
- Market Data
- MCP
---
