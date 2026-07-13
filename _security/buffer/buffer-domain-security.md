---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buffer.com
  spf: true
hosts:
- cert_expires: Sep 30 19:17:12 2026 GMT
  host: buffer.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:28:49 2026 GMT
  host: developers.buffer.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:28:49 2026 GMT
  host: api.buffer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buffer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buffer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Buffer
provider_slug: buffer
slug: buffer-domain-security
source_filename: buffer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.buffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:28:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.buffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:28:49 2026 GMT\n  hsts: null\ndomains:\n- domain: buffer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buffer/refs/heads/main/security/buffer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Scheduling
- Analytics
- Publishing
- Content Management
---
