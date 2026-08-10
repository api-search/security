---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zerocater.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: zerocater.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: app.zerocater.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zerocater Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zerocater, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zerocater
provider_slug: zerocater
slug: zerocater-domain-security
source_filename: zerocater-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zerocater.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.zerocater.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zerocater.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerocater/refs/heads/main/security/zerocater-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Catering
- Corporate Services
- Workplace
- Food Delivery
- Hospitality
- Artificial Intelligence
- Ordering
- Marketplace
---
