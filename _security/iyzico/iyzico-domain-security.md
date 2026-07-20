---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iyzico.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iyzipay.com
  spf: true
hosts:
- cert_expires: Oct  5 04:35:12 2026 GMT
  host: www.iyzico.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:12:42 2026 GMT
  host: docs.iyzico.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.iyzipay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Iyzico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iyzico, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Iyzico
provider_slug: iyzico
slug: iyzico-domain-security
source_filename: iyzico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iyzico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:35:12 2026 GMT\n  hsts: false\n- host: docs.iyzico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.iyzipay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iyzico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: iyzipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iyzico/refs/heads/main/security/iyzico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- FinTech
- Payment Gateway
- Card Payments
- Checkout
- Subscriptions
- Marketplace
- Turkey
- 3D Secure
---
