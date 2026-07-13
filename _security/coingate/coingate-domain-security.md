---
api_specs:
- filename: openapi.json
  format: json
  label: CoinGate Payment Gateway API
  slug: coingate-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coingate/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coingate.com
  spf: true
hosts:
- cert_expires: Oct  2 12:28:34 2026 GMT
  host: coingate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:02:52 2026 GMT
  host: developer.coingate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:28:34 2026 GMT
  host: api.coingate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coingate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinGate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoinGate
provider_slug: coingate
slug: coingate-domain-security
source_filename: coingate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coingate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.coingate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coingate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coingate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coingate/refs/heads/main/security/coingate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Payments
- Payment Gateway
- Crypto
- Fintech
- Bitcoin
- Ethereum
- Merchant Services
---
