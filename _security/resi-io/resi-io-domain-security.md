---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resi.io
  spf: true
hosts:
- cert_expires: Jan  7 16:19:49 2027 GMT
  host: resi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Resi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Resi
provider_slug: resi-io
slug: resi-io-domain-security
source_filename: resi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:19:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: resi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/resi-io/security/resi-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Streaming
- Video
- Live
- Encoding
---
