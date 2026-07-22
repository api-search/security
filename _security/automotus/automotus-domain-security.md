---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: automotus.ai
  spf: true
hosts:
- cert_expires: Aug 31 11:08:31 2026 GMT
  host: www.automotus.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automotus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automotus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Automotus
provider_slug: automotus
slug: automotus-domain-security
source_filename: automotus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.automotus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:08:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: automotus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automotus/refs/heads/main/security/automotus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Cities
- Urban Mobility
- Curb Management
- Computer Vision
- Transportation
- Parking
- Enforcement
---
