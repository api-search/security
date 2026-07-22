---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: timetric.com
  spf: false
hosts:
- cert_expires: Aug 28 02:41:28 2026 GMT
  host: www.timetric.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timetric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timetric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Timetric
provider_slug: timetric
slug: timetric-domain-security
source_filename: timetric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:41:28 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: timetric.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timetric/refs/heads/main/security/timetric-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data
- Time Series
- Analytics
- Market Research
- Financial Data
- Defunct
---
