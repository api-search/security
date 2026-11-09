---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caddence.golf
  spf: false
hosts:
- cert_expires: Jan 16 19:42:37 2027 GMT
  host: caddence.golf
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caddence Golf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caddence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Caddence
provider_slug: caddence-golf
slug: caddence-golf-domain-security
source_filename: caddence-golf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caddence.golf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 19:42:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: caddence.golf\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/caddence-golf/security/caddence-golf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Golf
- Price Comparison
- Retail
- Data Analytics
- United Kingdom
---
