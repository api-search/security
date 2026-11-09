---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 80l.app
  spf: true
hosts:
- cert_expires: Dec 20 20:55:45 2026 GMT
  host: 80l.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 80L App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eighty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eighty
provider_slug: 80l-app
slug: 80l-app-domain-security
source_filename: 80l-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 80l.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 20:55:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 80l.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/80l-app/security/80l-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Productivity
- Gamification
- Lifestyle
- Mobile
- RPG
---
