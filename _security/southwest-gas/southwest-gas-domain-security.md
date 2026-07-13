---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swgas.com
  spf: true
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.swgas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: myaccount.swgas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: agency.swgas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Southwest Gas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southwest Gas, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Southwest Gas
provider_slug: southwest-gas
slug: southwest-gas-domain-security
source_filename: southwest-gas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swgas.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myaccount.swgas.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agency.swgas.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swgas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southwest-gas/refs/heads/main/security/southwest-gas-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fortune 1000
- Natural Gas
- Utility
- Energy
---
