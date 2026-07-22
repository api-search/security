---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amperos.com
  spf: true
hosts:
- cert_expires: Sep 16 08:03:07 2026 GMT
  host: www.amperos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amperos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amperos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amperos
provider_slug: amperos
slug: amperos-domain-security
source_filename: amperos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amperos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amperos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amperos/refs/heads/main/security/amperos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Healthcare
- Revenue Cycle Management
- Insurance Claims
- Agentic AI
- Health Tech
- Denial Management
---
