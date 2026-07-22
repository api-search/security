---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spread.ai
  spf: true
hosts:
- cert_expires: Sep 11 23:53:43 2026 GMT
  host: spread.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPREAD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SPREAD
provider_slug: spread
slug: spread-domain-security
source_filename: spread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spread.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spread.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spread/refs/heads/main/security/spread-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Engineering Intelligence
- Product Lifecycle Management
- Manufacturing
- Automotive
- Low Code
- AI
---
