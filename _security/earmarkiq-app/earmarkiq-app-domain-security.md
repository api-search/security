---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: earmarkiq.app
  spf: true
hosts:
- cert_expires: Jan 23 06:04:22 2027 GMT
  host: earmarkiq.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earmarkiq App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for earmarkIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: earmarkIQ
provider_slug: earmarkiq-app
slug: earmarkiq-app-domain-security
source_filename: earmarkiq-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earmarkiq.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 06:04:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: earmarkiq.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/earmarkiq-app/security/earmarkiq-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Finance
- Artificial Intelligence
- Budgeting
- United Kingdom
---
