---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getcourt.co
  spf: true
hosts:
- cert_expires: Feb  4 00:44:09 2027 GMT
  host: getcourt.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GetCourt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetCourt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GetCourt
provider_slug: getcourt-co
slug: getcourt-co-domain-security
source_filename: getcourt-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcourt.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 00:44:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getcourt.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getcourt-co/security/getcourt-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports
- Community
- Tennis
- Padel
- Table Tennis
- Squash
- Platform
---
