---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cambrio.com
  spf: true
hosts:
- cert_expires: Nov 16 14:05:03 2026 GMT
  host: www.cambrio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cambrio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambrio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cambrio
provider_slug: cambrio
slug: cambrio-domain-security
source_filename: cambrio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cambrio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 14:05:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cambrio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambrio/refs/heads/main/security/cambrio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- CAD
- CAM
- CNC
- Manufacturing Software
- Digital Manufacturing
- Sandvik
---
