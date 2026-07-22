---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boosters.kr
  spf: false
hosts:
- cert_expires: Sep  6 08:37:56 2026 GMT
  host: en.boosters.kr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boosters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boosters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Boosters
provider_slug: boosters
slug: boosters-domain-security
source_filename: boosters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.boosters.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:37:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boosters.kr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boosters/refs/heads/main/security/boosters-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Commerce
- E-commerce
- K-Beauty
- D2C
- Brand Aggregator
- Korea
---
