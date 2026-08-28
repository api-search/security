---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: menusifu.com
  spf: true
hosts:
- cert_expires: Nov  3 11:29:15 2026 GMT
  host: www.menusifu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: api.menusifu.com
  hsts: false
  hsts_max_age: null
  https: true
  note: 'Production API host, added by hand — it is not named in apis.yml apis[] because MenuSifu publishes no API entry. Probed 2026-08-25: HTTP/2, no Strict-Transport-Security header, x-content-type-options nosniff and x-frame-options DENY present; highest TLS version negotiated by openssl s_client was TLSv1.2.'
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Menusifu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MenuSifu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MenuSifu
provider_slug: menusifu
slug: menusifu-domain-security
source_filename: menusifu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; api.menusifu.com probed directly 2026-08-25\nhosts:\n- host: www.menusifu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 11:29:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.menusifu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  cert_issuer: Amazon RSA 2048 M04\n  hsts: false\n  hsts_max_age: null\n  note: 'Production API host, added by hand — it is not named in apis.yml apis[] because MenuSifu publishes\n    no API entry. Probed 2026-08-25: HTTP/2, no Strict-Transport-Security header, x-content-type-options\n    nosniff and x-frame-options DENY present; highest TLS version negotiated by openssl s_client was TLSv1.2.'\ndomains:\n- domain: menusifu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/menusifu/refs/heads/main/security/menusifu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Point of Sale
- Restaurants
- Restaurant Technology
- Hospitality
- Payments
- Online Ordering
- Loyalty
- Kitchen Display Systems
- Hardware
---
