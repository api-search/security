---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tuas.com.au
  spf: false
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: tuas.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tuas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tuas
provider_slug: tuas
slug: tuas-domain-security
source_filename: tuas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tuas.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tuas.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuas/refs/heads/main/security/tuas-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Telecommunications
- Mobile
- Singapore
- Australia
- ASX Listed
---
