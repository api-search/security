---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ceta.cc
  spf: false
hosts:
- cert_expires: Oct  9 14:57:13 2026 GMT
  host: ceta.cc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ceta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ceta
provider_slug: ceta
slug: ceta-domain-security
source_filename: ceta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceta.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:57:13 2026 GMT\n  hsts: null\ndomains:\n- domain: ceta.cc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceta/refs/heads/main/security/ceta-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
