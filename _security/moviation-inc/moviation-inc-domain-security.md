---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: moviationair.com
  spf: true
hosts:
- cert_expires: Sep  5 06:05:42 2026 GMT
  host: www.moviationair.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moviation Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moviation, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Moviation, Inc.
provider_slug: moviation-inc
slug: moviation-inc-domain-security
source_filename: moviation-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moviationair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 06:05:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moviationair.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moviation-inc/refs/heads/main/security/moviation-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mobility
- Air Taxi
- Urban Air Mobility
- eVTOL
- Aviation
- Luxury Travel
- Transportation
---
