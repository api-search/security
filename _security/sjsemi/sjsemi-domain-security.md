---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sjsemi.com
  spf: true
hosts:
- cert_expires: Nov 15 02:18:36 2026 GMT
  host: en.sjsemi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sjsemi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SJSemi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SJSemi
provider_slug: sjsemi
slug: sjsemi-domain-security
source_filename: sjsemi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.sjsemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 02:18:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sjsemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sjsemi/refs/heads/main/security/sjsemi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductors
- Hardware
- Manufacturing
- Advanced Packaging
- Wafer Test
- OSAT
- China
---
