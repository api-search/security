---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carnotcompression.com
  spf: true
hosts:
- cert_expires: Dec  5 04:17:31 2026 GMT
  host: carnotcompression.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carnotcompression Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carnotcompression, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Carnotcompression
provider_slug: carnotcompression
slug: carnotcompression-domain-security
source_filename: carnotcompression-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carnotcompression.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 04:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: carnotcompression.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnotcompression/refs/heads/main/security/carnotcompression-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compression
- Energy
- Cleantech
- Manufacturing
---
