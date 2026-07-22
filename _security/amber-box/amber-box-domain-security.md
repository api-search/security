---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amberbox.com
  spf: true
hosts:
- cert_expires: Aug 21 02:17:42 2026 GMT
  host: amberbox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amber Box Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amber Box, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amber Box
provider_slug: amber-box
slug: amber-box-domain-security
source_filename: amber-box-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amberbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 02:17:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amberbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-box/refs/heads/main/security/amber-box-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Security
- Gunshot Detection
- Life Safety
- IoT
- Sensors
- Public Safety
---
