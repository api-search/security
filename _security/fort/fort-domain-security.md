---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fort.cx
  spf: false
hosts:
- cert_expires: Sep 22 03:04:24 2026 GMT
  host: fort.cx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fort Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fort, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Fort
provider_slug: fort
slug: fort-domain-security
source_filename: fort-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fort.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fort.cx\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fort/refs/heads/main/security/fort-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wearables
- Health
- Fitness
- Strength Training
- Consumer Hardware
- Longevity
- IoT
---
