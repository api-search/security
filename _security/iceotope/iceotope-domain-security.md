---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iceotope.com
  spf: true
hosts:
- cert_expires: Sep 27 15:02:52 2026 GMT
  host: www.iceotope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iceotope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iceotope, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Iceotope
provider_slug: iceotope
slug: iceotope-domain-security
source_filename: iceotope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iceotope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iceotope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iceotope/refs/heads/main/security/iceotope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Centers
- Liquid Cooling
- Thermal Management
- Infrastructure
- Edge Computing
- High Performance Computing
- Sustainability
- Hardware
---
