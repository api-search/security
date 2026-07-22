---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dyndrite.com
  spf: true
hosts:
- cert_expires: Aug 23 00:13:08 2026 GMT
  host: www.dyndrite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dyndrite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyndrite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dyndrite
provider_slug: dyndrite
slug: dyndrite-domain-security
source_filename: dyndrite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dyndrite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:13:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dyndrite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyndrite/refs/heads/main/security/dyndrite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Additive Manufacturing
- 3D Printing
- Digital Manufacturing
- Manufacturing Automation
- GPU Computing
- Toolpathing
---
