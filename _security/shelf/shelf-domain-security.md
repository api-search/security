---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shelf.io
  spf: true
hosts:
- cert_expires: Aug 11 14:26:14 2026 GMT
  host: shelf.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shelf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shelf.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shelf.io
provider_slug: shelf
slug: shelf-domain-security
source_filename: shelf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shelf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 14:26:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shelf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shelf/refs/heads/main/security/shelf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Contact Center
- Knowledge Management
- SaaS
- Search
---
