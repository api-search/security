---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lmk.today
  spf: true
hosts:
- cert_expires: Dec 19 19:29:49 2026 GMT
  host: lmk.today
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LMK.today Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LMK.today, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LMK.today
provider_slug: lmk-today
slug: lmk-today-domain-security
source_filename: lmk-today-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lmk.today\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 19:29:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lmk.today\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lmk-today/security/lmk-today-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wishlist
- Price-Tracker
- E-Commerce
- Affiliates
- AI-Extension
---
