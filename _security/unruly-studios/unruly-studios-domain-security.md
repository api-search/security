---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unrulysplats.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unruly-studios.com
  spf: true
hosts:
- cert_expires: Oct  4 10:13:04 2026 GMT
  host: www.unrulysplats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: status.unrulysplats.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 15:51:21 2026 GMT
  host: gamelocker.unruly-studios.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unruly Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unruly Studios, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Unruly Studios
provider_slug: unruly-studios
slug: unruly-studios-domain-security
source_filename: unruly-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unrulysplats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:13:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.unrulysplats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: gamelocker.unruly-studios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 15:51:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: unrulysplats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: unruly-studios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unruly-studios/refs/heads/main/security/unruly-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- STEM
- EdTech
- Coding
- Kids
- Learning
- Hardware
---
