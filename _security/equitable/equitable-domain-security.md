---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: equitable.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: equitable.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api.equitable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equitable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equitable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Equitable
provider_slug: equitable
slug: equitable-domain-security
source_filename: equitable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equitable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.equitable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: equitable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equitable/refs/heads/main/security/equitable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benefits
- Financial Services
- Insurance
- Retirement
- Employee Benefits
---
