---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tripplus.cc
  spf: true
hosts:
- cert_expires: Sep  4 22:07:29 2026 GMT
  host: tripplus.cc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripplus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripplus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tripplus
provider_slug: tripplus
slug: tripplus-domain-security
source_filename: tripplus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripplus.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:07:29 2026 GMT\n  hsts: null\ndomains:\n- domain: tripplus.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripplus/refs/heads/main/security/tripplus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Loyalty
- Rewards
- Points
- Miles
- Credit Cards
- Fintech
- Taiwan
---
