---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heva.co
  spf: true
hosts:
- cert_expires: Aug 26 00:36:43 2026 GMT
  host: heva.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for heva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: heva
provider_slug: heva
slug: heva-domain-security
source_filename: heva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heva.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:36:43 2026 GMT\n  hsts: false\ndomains:\n- domain: heva.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heva/refs/heads/main/security/heva-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Tourism
- Practice Management
- Appointment Booking
- Artificial Intelligence
- Payments
- Cross-Border Care
- Health Tech
---
