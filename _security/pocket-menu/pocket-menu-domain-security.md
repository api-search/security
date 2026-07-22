---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pocket-concierge.jp
  spf: false
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: pocket-concierge.jp
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pocket Menu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pocket Menu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pocket Menu
provider_slug: pocket-menu
slug: pocket-menu-domain-security
source_filename: pocket-menu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pocket-concierge.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: pocket-concierge.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocket-menu/refs/heads/main/security/pocket-menu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Restaurants
- Reservations
- Payments
- Dining
- Hospitality
- Japan
---
