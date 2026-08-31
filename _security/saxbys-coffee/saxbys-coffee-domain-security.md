---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saxbyscoffee.com
  spf: true
hosts:
- cert_expires: Sep 16 02:31:38 2026 GMT
  host: www.saxbyscoffee.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saxbys Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saxbys Coffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Saxbys Coffee
provider_slug: saxbys-coffee
slug: saxbys-coffee-domain-security
source_filename: saxbys-coffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saxbyscoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:31:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: saxbyscoffee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saxbys-coffee/refs/heads/main/security/saxbys-coffee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coffee
- Cafe
- Hospitality
- Food And Beverage
- Quick Service Restaurant
- Education
- Experiential Learning
- Higher Education
- Student Run Business
- Retail
- Philadelphia
- Private Company
- No Public API
---
