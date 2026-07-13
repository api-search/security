---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reyrey.com
  spf: true
hosts:
- cert_expires: Sep 30 22:04:04 2026 GMT
  host: www.reyrey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reynolds Reynolds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reynolds and Reynolds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reynolds and Reynolds
provider_slug: reynolds-reynolds
slug: reynolds-reynolds-domain-security
source_filename: reynolds-reynolds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reyrey.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 22:04:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reyrey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reynolds-reynolds/refs/heads/main/security/reynolds-reynolds-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Automotive
- Dealership Management System
- DMS
- Reynolds Certified Interface
- RCI
- Certified Interface
- Partner API
- Gated Access
---
