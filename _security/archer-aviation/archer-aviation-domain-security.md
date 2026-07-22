---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archer.com
  spf: true
hosts:
- cert_expires: Sep 14 05:37:35 2026 GMT
  host: www.archer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:42:58 2026 GMT
  host: defense.archer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archer Aviation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archer Aviation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Archer Aviation
provider_slug: archer-aviation
slug: archer-aviation-domain-security
source_filename: archer-aviation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.archer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:37:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: defense.archer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:42:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: archer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archer-aviation/refs/heads/main/security/archer-aviation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advanced Air Mobility
- Aerospace
- Air Taxi
- Defense
- eVTOL
- Electric Aviation
- FAA Certification
- Manufacturing
- Sustainable Aviation
- Urban Air Mobility
---
