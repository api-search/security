---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pixyalbum.com
  spf: true
hosts:
- cert_expires: Sep  2 02:05:18 2026 GMT
  host: pixyalbum.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixyalbum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixyalbum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pixyalbum
provider_slug: pixyalbum
slug: pixyalbum-domain-security
source_filename: pixyalbum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixyalbum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: pixyalbum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixyalbum/refs/heads/main/security/pixyalbum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Photo Printing
- Photo Books
- Consumer
- E-commerce
- Printing
- Mexico
- Photography
---
