---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: planka.app
  spf: true
hosts:
- cert_expires: Jan 18 04:52:20 2027 GMT
  host: planka.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Planka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PLANKA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PLANKA
provider_slug: planka
slug: planka-domain-security
source_filename: planka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planka.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 04:52:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: planka.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/planka/security/planka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kanban
- Project Management
- Self-Hosted
- Agile
- Open Source
---
