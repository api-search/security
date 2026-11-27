---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getcallme.app
  spf: true
hosts:
- cert_expires: Dec 20 19:47:04 2026 GMT
  host: getcallme.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Call Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Call Me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Call Me
provider_slug: getcallme-app
slug: getcallme-app-domain-security
source_filename: getcallme-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcallme.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 19:47:04 2026 GMT\n  hsts: false\ndomains:\n- domain: getcallme.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getcallme-app/security/getcallme-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Assistant
- Productivity
- Voice
- Software-as-a-Service
---
