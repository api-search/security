---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coastpay.com
  spf: true
hosts:
- cert_expires: Oct 11 18:05:51 2026 GMT
  host: coastpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 18:52:49 2026 GMT
  host: developers.coastpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.coastpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coast Fka Vayu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coast (FKA VayU), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coast (FKA VayU)
provider_slug: coast-fka-vayu
slug: coast-fka-vayu-domain-security
source_filename: coast-fka-vayu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coastpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:05:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.coastpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coastpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coastpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coast-fka-vayu/refs/heads/main/security/coast-fka-vayu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fleet Cards
- Fuel Cards
- Corporate Cards
- Expense Management
- Fintech
- Bill Pay
---
