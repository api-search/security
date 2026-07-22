---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pulsespace.com
  spf: true
hosts:
- cert_expires: Sep  6 01:59:50 2026 GMT
  host: pulsespace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulse Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pulse Space
provider_slug: pulse-space
slug: pulse-space-domain-security
source_filename: pulse-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulsespace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:59:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pulsespace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-space/refs/heads/main/security/pulse-space-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Space
- Aerospace
- Satellites
- Power
- Energy
- Hardware
- Techstars
---
