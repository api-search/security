---
api_specs:
- filename: overview
  format: yaml
  label: TronZap REST API
  slug: tronzap-rest-api
  spec_type: Postman
  url: https://www.postman.com/tron-energy/tronzap-com/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tronzap.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: docs.tronzap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.tronzap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tronzap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TronZap, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TronZap
provider_slug: tronzap
slug: tronzap-domain-security
source_filename: tronzap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.tronzap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\n- host: api.tronzap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tronzap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronzap/refs/heads/main/security/tronzap-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- TRON
- DeFi infrastructure
- Stablecoins
- USDT
- TRC-20
- Resource marketplace
- Payments
- Fees optimization
- Web3
- DeFi
- Payouts
- Compliance
- AML
- Developer Tools
- SDK
---
