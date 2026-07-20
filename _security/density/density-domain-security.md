---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: density.io
  spf: true
hosts:
- cert_expires: Oct 14 12:33:56 2026 GMT
  host: www.density.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:01:51 2026 GMT
  host: developers.density.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: api.density.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Density Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Density, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Density
provider_slug: density
slug: density-domain-security
source_filename: density-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.density.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.density.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.density.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: density.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/density/refs/heads/main/security/density-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Occupancy Sensors
- Workplace Analytics
- Real Time
- Occupancy
- Sensors
- IoT
- Space Utilization
- Proptech
---
