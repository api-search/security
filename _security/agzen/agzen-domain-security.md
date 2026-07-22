---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agzen.com
  spf: false
hosts:
- cert_expires: Aug 21 08:28:59 2026 GMT
  host: www.agzen.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agzen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgZen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AgZen
provider_slug: agzen
slug: agzen-domain-security
source_filename: agzen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:28:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: agzen.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agzen/refs/heads/main/security/agzen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Precision Agriculture
- Computer Vision
- Artificial Intelligence
- Crop Protection
- Sensors
- Sustainability
---
