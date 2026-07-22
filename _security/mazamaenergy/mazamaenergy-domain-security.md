---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mazamaenergy.com
  spf: true
hosts:
- cert_expires: Sep 25 14:44:06 2026 GMT
  host: mazamaenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mazamaenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mazama Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mazama Energy
provider_slug: mazamaenergy
slug: mazamaenergy-domain-security
source_filename: mazamaenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mazamaenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:44:06 2026 GMT\n  hsts: false\ndomains:\n- domain: mazamaenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mazamaenergy/refs/heads/main/security/mazamaenergy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Geothermal
- Clean Energy
- Renewable Energy
- Enhanced Geothermal Systems
- Power Generation
- Climate Tech
---
