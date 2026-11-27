---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reelmint.io
  spf: false
hosts:
- cert_expires: Jan 29 11:14:34 2027 GMT
  host: reelmint.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReelMint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReelMint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ReelMint
provider_slug: reelmint-io
slug: reelmint-io-domain-security
source_filename: reelmint-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reelmint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 11:14:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reelmint.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reelmint-io/security/reelmint-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- AI
- Shorts
- MCP
- Studio
---
