---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ateios.com
  spf: true
hosts:
- cert_expires: Sep  4 22:33:05 2026 GMT
  host: ateios.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ateios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ateios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ateios
provider_slug: ateios
slug: ateios-domain-security
source_filename: ateios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ateios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:33:05 2026 GMT\n  hsts: false\ndomains:\n- domain: ateios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ateios/refs/heads/main/security/ateios-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Batteries
- Energy Storage
- Battery Materials
- Manufacturing
- Cleantech
- Hardware
---
