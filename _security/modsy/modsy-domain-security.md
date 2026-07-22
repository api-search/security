---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: modsy.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.modsy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modsy *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Modsy *
provider_slug: modsy
slug: modsy-domain-security
source_filename: modsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modsy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modsy/refs/heads/main/security/modsy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Interior Design
- 3D Visualization
- Home
- Real Estate
---
