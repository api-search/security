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
- cert_expires: Sep 20 20:01:28 2026 GMT
  host: docs.coastpay.com
  hsts: null
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
name: Coast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coast
provider_slug: coast
slug: coast-domain-security
source_filename: coast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coastpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:05:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coastpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:01:28 2026 GMT\n  hsts: null\n- host: api.coastpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coastpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coast/refs/heads/main/security/coast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Fleet
- Fuel Cards
- Corporate Cards
- Expense Management
- Bill Pay
---
