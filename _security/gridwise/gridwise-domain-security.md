---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gridwise.io
  spf: true
hosts:
- cert_expires: Oct 12 19:36:06 2026 GMT
  host: gridwise.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gridwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gridwise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gridwise
provider_slug: gridwise
slug: gridwise-domain-security
source_filename: gridwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gridwise.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:36:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gridwise.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridwise/refs/heads/main/security/gridwise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gig Economy
- Rideshare
- Delivery
- Mobility Data
- Analytics
- Earnings Tracking
- Data Products
---
