---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: peek.com
  spf: true
hosts:
- cert_expires: Oct  4 14:43:26 2026 GMT
  host: www.peek.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 03:01:20 2026 GMT
  host: octodocs.peek.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 14:37:42 2027 GMT
  host: octo.peek.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peek, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Peek
provider_slug: peek
slug: peek-domain-security
source_filename: peek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:43:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: octodocs.peek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 03:01:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: octo.peek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 14:37:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peek/refs/heads/main/security/peek-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Tourism
- Booking
- Reservations
- Experiences
- Tours and Activities
- Payments
- Marketplace
- MCP
- OCTO
- SaaS
---
