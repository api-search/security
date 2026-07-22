---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wibmo.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: wibmo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 10:29:40 2026 GMT
  host: developer.wibmo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wibmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WIBMO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: WIBMO
provider_slug: wibmo
slug: wibmo-domain-security
source_filename: wibmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wibmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wibmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:29:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wibmo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wibmo/refs/heads/main/security/wibmo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Payments
- Fintech
- Payment Gateway
- Tokenization
- Fraud Detection
- 3-D Secure
- Authentication
- Digital Wallet
- Prepaid Cards
- India
---
