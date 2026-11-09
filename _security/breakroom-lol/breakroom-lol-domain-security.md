---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: breakroom.lol
  spf: true
hosts:
- cert_expires: Dec 31 07:08:37 2026 GMT
  host: breakroom.lol
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breakroom Lol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Break Room, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Break Room
provider_slug: breakroom-lol
slug: breakroom-lol-domain-security
source_filename: breakroom-lol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breakroom.lol\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 07:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: breakroom.lol\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/breakroom-lol/security/breakroom-lol-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Gaming
- Artificial Intelligence
- Agents
- Multiplayer
- OpenAPI
---
