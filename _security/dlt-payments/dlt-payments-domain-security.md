---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dltpay.com
  spf: false
hosts:
- cert_expires: Sep 27 20:17:21 2026 GMT
  host: dltpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dlt Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DLT Payments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DLT Payments
provider_slug: dlt-payments
slug: dlt-payments-domain-security
source_filename: dlt-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dltpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:17:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dltpay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dlt-payments/refs/heads/main/security/dlt-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Stablecoin
- Cryptocurrency
- Blockchain
- Web3
- Wallet
- Fintech
---
