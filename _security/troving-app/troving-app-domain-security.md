---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: troving.app
  spf: false
hosts:
- cert_expires: Jan  4 14:23:59 2027 GMT
  host: troving.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trove
provider_slug: troving-app
slug: troving-app-domain-security
source_filename: troving-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: troving.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 14:23:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: troving.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/troving-app/security/troving-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Productivity
- ADHD
- Task Management
- AI Assistants
---
