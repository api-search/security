---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: picktrace.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: picktrace.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Picktrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PickTrace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PickTrace
provider_slug: picktrace
slug: picktrace-domain-security
source_filename: picktrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: picktrace.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: picktrace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picktrace/refs/heads/main/security/picktrace-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Agriculture
- AgTech
- Workforce Management
- Labor Tracking
- Farm Management
- Harvest Management
- Time Tracking
- Payroll
- Piecework
- API
---
