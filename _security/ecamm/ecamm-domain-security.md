---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecamm.com
  spf: true
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: ecamm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ecamm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecamm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ecamm
provider_slug: ecamm
slug: ecamm-domain-security
source_filename: ecamm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecamm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ecamm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecamm/security/ecamm-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Live Streaming
- Video Production
- Multistreaming
- Virtual Camera
- Screen Capture
- Guest Video
---
