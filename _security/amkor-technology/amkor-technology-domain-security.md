---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amkor.com
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.amkor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amkor Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amkor Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amkor Technology
provider_slug: amkor-technology
slug: amkor-technology-domain-security
source_filename: amkor-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amkor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amkor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amkor-technology/refs/heads/main/security/amkor-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Semiconductor Packaging
- OSAT
- Test Services
- Advanced Packaging
- Chiplets
- Automotive
- Artificial Intelligence
- Electronics Manufacturing
- Fortune 1000
---
