---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: memebo.at
  spf: false
hosts:
- cert_expires: Jan  6 20:38:02 2027 GMT
  host: memebo.at
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memeboat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memeboat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Memeboat
provider_slug: memebo-at
slug: memebo-at-domain-security
source_filename: memebo-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memebo.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 20:38:02 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: memebo.at\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/memebo-at/security/memebo-at-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Meme Generator
- Free
- Anonymous
- Online
- Creative
---
