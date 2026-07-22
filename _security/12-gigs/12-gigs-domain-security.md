---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superluckycasino.com
  spf: true
hosts:
- cert_expires: Sep 13 15:51:11 2026 GMT
  host: superluckycasino.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 12 Gigs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 12 Gigs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 12 Gigs
provider_slug: 12-gigs
slug: 12-gigs-domain-security
source_filename: 12-gigs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superluckycasino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:51:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: superluckycasino.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/12-gigs/refs/heads/main/security/12-gigs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Mobile Games
- Social Casino
- Casual Games
- Word Games
- Stillfront
---
