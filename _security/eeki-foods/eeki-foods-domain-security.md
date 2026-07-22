---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eekifoods.com
  spf: false
hosts:
- cert_expires: Aug 19 14:39:08 2026 GMT
  host: www.eekifoods.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eeki Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eeki Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Eeki Foods
provider_slug: eeki-foods
slug: eeki-foods-domain-security
source_filename: eeki-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eekifoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:39:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eekifoods.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eeki-foods/refs/heads/main/security/eeki-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food and Beverage
- Food
- Portfolio Company
- Venture Backed
- General Catalyst
- Pre-Launch
---
