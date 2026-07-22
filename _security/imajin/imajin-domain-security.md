---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imajin.id
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: imajin.id
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imajin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imajin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Imajin
provider_slug: imajin
slug: imajin-domain-security
source_filename: imajin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imajin.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: imajin.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imajin/refs/heads/main/security/imajin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Marketplace
- 3D Printing
- Prototyping
- CNC Machining
- Mold and Die
- Mass Production
- Fabrication
- Indonesia
- B2B
---
