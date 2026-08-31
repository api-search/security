---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: examedi.com
  spf: true
hosts:
- cert_expires: Sep 19 06:01:51 2026 GMT
  host: examedi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.examedi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Examedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Examedi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Examedi
provider_slug: examedi
slug: examedi-domain-security
source_filename: examedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: examedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.examedi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: examedi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/examedi/refs/heads/main/security/examedi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- HealthTech
- Diagnostics
- Laboratory
- Medical Testing
- At-Home Care
- Latin America
---
