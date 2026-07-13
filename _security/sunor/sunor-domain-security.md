---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sunor.cc
  spf: true
hosts:
- cert_expires: Oct  6 07:41:50 2026 GMT
  host: docs.sunor.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sunor
provider_slug: sunor
slug: sunor-domain-security
source_filename: sunor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sunor.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:41:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sunor.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunor/refs/heads/main/security/sunor-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Music
- Public APIs
---
