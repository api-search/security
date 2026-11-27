---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: epochcalc.com
  spf: false
hosts:
- cert_expires: Dec 28 00:14:52 2026 GMT
  host: epochcalc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Epoch Calculator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epoch Calculator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Epoch Calculator
provider_slug: epochcalc-com
slug: epochcalc-com-domain-security
source_filename: epochcalc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epochcalc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 00:14:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epochcalc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/epochcalc-com/security/epochcalc-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Time
- Utilities
- JavaScript
- Free
- Open Source
---
