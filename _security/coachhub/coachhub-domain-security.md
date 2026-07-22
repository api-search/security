---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coachhub.io
  spf: true
hosts:
- cert_expires: Aug 10 21:05:37 2026 GMT
  host: coachhub.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coachhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for coachhub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: coachhub
provider_slug: coachhub
slug: coachhub-domain-security
source_filename: coachhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coachhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 21:05:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coachhub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coachhub/refs/heads/main/security/coachhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Digital Coaching
- Learning And Development
- HR Tech
- Employee Development
- SaaS
---
