---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boringstuff.club
  spf: true
hosts:
- cert_expires: Jan 17 18:29:48 2027 GMT
  host: boringstuff.club
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boringstuff Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boring Stuff Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boring Stuff Club
provider_slug: boringstuff-club
slug: boringstuff-club-domain-security
source_filename: boringstuff-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boringstuff.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 18:29:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boringstuff.club\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/boringstuff-club/security/boringstuff-club-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animation
- Illustration
- Product Demo
- Education
---
