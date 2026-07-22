---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glorify.global
  spf: false
hosts:
- cert_expires: Sep 13 00:30:09 2026 GMT
  host: www.glorify.global
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glorify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glorify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Glorify
provider_slug: glorify
slug: glorify-domain-security
source_filename: glorify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glorify.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:30:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glorify.global\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glorify/refs/heads/main/security/glorify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Religion
- Faith
- Devotional
- Wellness
- Meditation
- Christian
- Consumer App
---
