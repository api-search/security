---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: convenientpower.com
  spf: true
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: convenientpower.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Convenientpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConvenientPower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ConvenientPower
provider_slug: convenientpower
slug: convenientpower-domain-security
source_filename: convenientpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convenientpower.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: convenientpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convenientpower/refs/heads/main/security/convenientpower-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Semiconductor
- Wireless Charging
- Power Management
- USB Power Delivery
- Battery Management
- Automotive
- Integrated Circuits
---
