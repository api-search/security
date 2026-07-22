---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: masmovil.es
  spf: true
hosts:
- cert_expires: Sep 26 12:55:02 2026 GMT
  host: www.masmovil.es
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Masmovil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Masmovil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Masmovil
provider_slug: masmovil
slug: masmovil-domain-security
source_filename: masmovil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.masmovil.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:55:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: masmovil.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/masmovil/refs/heads/main/security/masmovil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Telecommunications
- Mobile
- Fiber
- Internet
- Spain
---
