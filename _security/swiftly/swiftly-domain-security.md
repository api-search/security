---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swiftly.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: swiftlyapi.net
  spf: false
hosts:
- cert_expires: Oct 11 15:12:17 2026 GMT
  host: swiftly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: prod.swiftlyapi.net
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiftly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swiftly, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swiftly
provider_slug: swiftly
slug: swiftly-domain-security
source_filename: swiftly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swiftly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 15:12:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod.swiftlyapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: swiftly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: swiftlyapi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftly/refs/heads/main/security/swiftly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Retail Media
- Grocery
- Advertising
- Loyalty
- Coupons
- Commerce
- Artificial Intelligence
- Mobile
- Company
---
