---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mismarapp.com
  spf: true
hosts:
- cert_expires: Sep  5 04:16:46 2026 GMT
  host: mismarapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mismar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MisMar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MisMar
provider_slug: mismar
slug: mismar-domain-security
source_filename: mismar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mismarapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:16:46 2026 GMT\n  hsts: false\ndomains:\n- domain: mismarapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mismar/refs/heads/main/security/mismar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Car Maintenance
- Vehicle Repair
- Fleet Management
- Workshop Management
- Mobile App
- Saudi Arabia
- Insurance
---
