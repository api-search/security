---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: artillery.io
  spf: true
hosts:
- cert_expires: Aug  9 20:50:05 2026 GMT
  host: www.artillery.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: app.artillery.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artillery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artillery, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Artillery
provider_slug: artillery
slug: artillery-domain-security
source_filename: artillery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artillery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 20:50:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.artillery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: artillery.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artillery/refs/heads/main/security/artillery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Load Testing
- Performance Testing
- Open Source
- Testing
- DevOps
- Node.js
---
