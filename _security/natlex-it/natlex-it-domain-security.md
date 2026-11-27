---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: natlex.it
  spf: true
hosts:
- cert_expires: Jan 16 14:15:23 2027 GMT
  host: natlex.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Natlex IT Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natlex IT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Natlex IT
provider_slug: natlex-it
slug: natlex-it-domain-security
source_filename: natlex-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: natlex.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 14:15:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: natlex.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/natlex-it/security/natlex-it-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Applications
- Nutrition app
- Voice recorder
- Astrology app
- Educational game
- Product Studio
- Mobile App
- B2B AI services
---
