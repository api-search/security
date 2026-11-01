---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: trypenny.com
  spf: true
hosts:
- cert_expires: Dec  2 04:54:57 2026 GMT
  host: trypenny.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Penny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penny, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Penny
provider_slug: penny
slug: penny-domain-security
source_filename: penny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trypenny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 04:54:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trypenny.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/penny/security/penny-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Fintech
- Retirement
- Pensions
- MobileApp
- FinancialPlanning
---
