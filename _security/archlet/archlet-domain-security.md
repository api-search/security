---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: archlet.io
  spf: false
hosts:
- cert_expires: Aug 23 17:46:20 2026 GMT
  host: archlet.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archlet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archlet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Archlet
provider_slug: archlet
slug: archlet-domain-security
source_filename: archlet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archlet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 17:46:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: archlet.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archlet/refs/heads/main/security/archlet-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Ai Enterprise Software
- Procurement
- Sourcing
- eSourcing
- eAuctions
- Sourcing Optimization
- Supply Chain
- Spend Management
- Enterprise Software
- Artificial Intelligence
---
