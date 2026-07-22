---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 4pillars.io
  spf: false
hosts:
- cert_expires: Aug 24 12:21:24 2026 GMT
  host: 4pillars.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Four Pillars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Four Pillars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Four Pillars
provider_slug: four-pillars
slug: four-pillars-domain-security
source_filename: four-pillars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4pillars.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:21:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 4pillars.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/four-pillars/refs/heads/main/security/four-pillars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Blockchain
- Research
- Validator
- Staking
- Advisory
- Asia
---
