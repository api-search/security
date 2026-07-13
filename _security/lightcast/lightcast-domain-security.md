---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lightcast.dev
  spf: false
hosts:
- cert_expires: Sep 21 02:11:33 2026 GMT
  host: docs.lightcast.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightcast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lightcast
provider_slug: lightcast
slug: lightcast-domain-security
source_filename: lightcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.lightcast.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:11:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lightcast.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightcast/refs/heads/main/security/lightcast-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Careers
- Economics
- Labor Market
- Workforce
---
