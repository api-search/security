---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: athletesfirst.net
  spf: true
hosts:
- cert_expires: Oct  6 19:09:58 2026 GMT
  host: www.athletesfirst.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athletes First Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athletes First, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Athletes First
provider_slug: athletes-first
slug: athletes-first-domain-security
source_filename: athletes-first-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.athletesfirst.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:09:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: athletesfirst.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletes-first/refs/heads/main/security/athletes-first-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Sports
- Sports Representation
- Talent Agency
- Athlete Management
- NFL
- Sports Marketing
---
