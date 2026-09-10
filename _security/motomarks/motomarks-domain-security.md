---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: motomarks.io
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: motomarks.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.motomarks.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Motomarks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motomarks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Motomarks
provider_slug: motomarks
slug: motomarks-domain-security
source_filename: motomarks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motomarks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.motomarks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: motomarks.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motomarks/refs/heads/main/security/motomarks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- automotive
- logo
- image-cdn
- manufacturer
- brand-assets
- images
- CDN
- developer-tools
- agent-native
- MCP
- reference-data
---
