---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: monetizr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: themonetizr.com
  spf: true
hosts:
- cert_expires: Sep 28 06:50:32 2026 GMT
  host: monetizr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:40:16 2026 GMT
  host: api.themonetizr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Themonetizr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheMonetizr, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TheMonetizr
provider_slug: themonetizr
slug: themonetizr-domain-security
source_filename: themonetizr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monetizr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:50:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.themonetizr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:40:16 2026 GMT\n  hsts: false\ndomains:\n- domain: monetizr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: themonetizr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/themonetizr/refs/heads/main/security/themonetizr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Gaming
- In-Game Advertising
- Monetization
- Mobile
- Rewards
- Ad Tech
- Programmatic
- Unity
---
