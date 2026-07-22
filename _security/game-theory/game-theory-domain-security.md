---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gametheory.in
  spf: true
hosts:
- cert_expires: Sep  9 14:17:33 2026 GMT
  host: gametheory.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Game Theory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Game Theory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Game Theory
provider_slug: game-theory
slug: game-theory-domain-security
source_filename: game-theory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gametheory.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:17:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gametheory.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/game-theory/refs/heads/main/security/game-theory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Fitness
- Recreation
- Membership
- Sports Coaching
- Mobile App
- Bengaluru
- India
- Techstars
---
