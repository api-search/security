---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memol.app
  spf: true
hosts:
- cert_expires: Feb  3 06:44:18 2027 GMT
  host: memol.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Memol
provider_slug: memol-app
slug: memol-app-domain-security
source_filename: memol-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memol.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 06:44:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memol.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/memol-app/security/memol-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notes
- AI Assistant
- Knowledge Management
- Task Management
- Migration
---
