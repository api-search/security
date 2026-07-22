---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pelikan-mobility.com
  spf: true
hosts:
- cert_expires: Oct  1 11:33:07 2026 GMT
  host: pelikan-mobility.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pelikan Mobility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pelikan Mobility, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pelikan Mobility
provider_slug: pelikan-mobility
slug: pelikan-mobility-domain-security
source_filename: pelikan-mobility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pelikan-mobility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:33:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pelikan-mobility.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pelikan-mobility/refs/heads/main/security/pelikan-mobility-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mobility
- Electric Vehicles
- Fleet Management
- Leasing
- Sustainability
---
