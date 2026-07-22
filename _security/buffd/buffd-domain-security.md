---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: buffd.gg
  spf: true
hosts:
- cert_expires: Sep 24 01:06:46 2026 GMT
  host: www.buffd.gg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buffd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buffd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Buffd
provider_slug: buffd
slug: buffd-domain-security
source_filename: buffd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buffd.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:06:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buffd.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buffd/refs/heads/main/security/buffd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Esports
- Consumer
- Progressive Web App
- Mobile
---
