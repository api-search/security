---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gravitysketch.com
  spf: true
hosts:
- cert_expires: Nov  1 05:13:51 2026 GMT
  host: www.gravitysketch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gravity Sketch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravity Sketch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gravity Sketch
provider_slug: gravity-sketch
slug: gravity-sketch-domain-security
source_filename: gravity-sketch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gravitysketch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 05:13:51 2026 GMT\n  hsts: false\ndomains:\n- domain: gravitysketch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravity-sketch/refs/heads/main/security/gravity-sketch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Design
- 3D Design
- Virtual Reality
- Product Design
- Automotive Design
- Collaboration
- Creative Tools
---
