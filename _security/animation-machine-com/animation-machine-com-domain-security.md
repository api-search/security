---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: animation-machine.com
  spf: false
hosts:
- cert_expires: Jan 14 06:02:40 2027 GMT
  host: animation-machine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Animation Machine Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cash Flow Crescendo Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cash Flow Crescendo Inc.
provider_slug: animation-machine-com
slug: animation-machine-com-domain-security
source_filename: animation-machine-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: animation-machine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:02:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: animation-machine.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/animation-machine-com/security/animation-machine-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animation
- Video
- Artificial Intelligence
- Conversion
- Software-as-a-Service
- Multimedia
---
