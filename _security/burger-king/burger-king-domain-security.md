---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bk.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.bk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Burger King Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burger King, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Burger King
provider_slug: burger-king
slug: burger-king-domain-security
source_filename: burger-king-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burger-king/refs/heads/main/security/burger-king-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fast Food
- Restaurants
- Food & Beverage
- Loyalty
- Mobile Ordering
---
