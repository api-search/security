---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: cycle.eco
  spf: true
hosts:
- cert_expires: Oct 15 02:20:18 2026 GMT
  host: cycle.eco
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cycle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Cycle
provider_slug: cycle
slug: cycle-domain-security
source_filename: cycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cycle.eco\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cycle.eco\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycle/refs/heads/main/security/cycle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Micromobility
- E-Bikes
- Urban Mobility
- Delivery
- Logistics
- Transportation
- Subscription
- Sustainability
- Fleet
---
