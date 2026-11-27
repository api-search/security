---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gol24.uz
  spf: true
hosts:
- cert_expires: Dec 20 09:30:07 2026 GMT
  host: gol24.uz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: gol24.uz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gol24.uz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: gol24.uz
provider_slug: gol24-uz
slug: gol24-uz-domain-security
source_filename: gol24-uz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gol24.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 09:30:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gol24.uz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gol24-uz/security/gol24-uz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Football
- News
- Uzbekistan
- Sports
---
