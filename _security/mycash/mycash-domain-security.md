---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: inremit.co
  spf: true
hosts:
- cert_expires: Oct  9 08:33:35 2026 GMT
  host: inremit.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mycash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyCash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MyCash
provider_slug: mycash
slug: mycash-domain-security
source_filename: mycash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inremit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:33:35 2026 GMT\n  hsts: null\ndomains:\n- domain: inremit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycash/refs/heads/main/security/mycash-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Remittance
- Payments
- Money Transfer
- Fintech
- Financial Services
- Mobile
- Cross-Border Payments
- Singapore
---
