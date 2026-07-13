---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coinlib.io
  spf: true
hosts:
- cert_expires: Aug 22 08:15:39 2026 GMT
  host: coinlib.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinlib Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinlib, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coinlib
provider_slug: coinlib
slug: coinlib-domain-security
source_filename: coinlib-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinlib.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:15:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coinlib.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinlib/refs/heads/main/security/coinlib-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cryptocurrency
- Public APIs
---
