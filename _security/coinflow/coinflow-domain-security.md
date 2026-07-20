---
api_specs:
- filename: coinflow-openapi-original.json
  format: json
  label: Coinflow API
  slug: coinflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinflow.cash
  spf: true
hosts:
- cert_expires: Oct  1 14:31:00 2026 GMT
  host: coinflow.cash
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 14:32:10 2026 GMT
  host: api-sandbox.coinflow.cash
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinflow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinflow
provider_slug: coinflow
slug: coinflow-domain-security
source_filename: coinflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinflow.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:31:00 2026 GMT\n  hsts: false\n- host: api-sandbox.coinflow.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:32:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coinflow.cash\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/security/coinflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Payments
- Stablecoin
- USDC
- Checkout
- Payouts
- Marketplace
- Web3
- Fintech
---
