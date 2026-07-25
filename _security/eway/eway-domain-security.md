---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eway.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eway.io
  spf: true
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.eway.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 00:37:54 2026 GMT
  host: eway.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: api.ewaypayments.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eWAY, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: eWAY
provider_slug: eway
slug: eway-domain-security
source_filename: eway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eway.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eway.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:37:54 2026 GMT\n  hsts: false\n- host: api.ewaypayments.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: eway.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eway.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eway/refs/heads/main/security/eway-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Card Payments
- Tokenization
- E-commerce
- Recurring Payments
- Subscriptions
---
