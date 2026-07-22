---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: happiestbaby.com
  spf: true
hosts:
- cert_expires: Sep 19 22:34:49 2026 GMT
  host: happiestbaby.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Happiest Baby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Happiest Baby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Happiest Baby
provider_slug: happiest-baby
slug: happiest-baby-domain-security
source_filename: happiest-baby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: happiestbaby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:34:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: happiestbaby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happiest-baby/refs/heads/main/security/happiest-baby-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Baby
- Sleep Technology
- Smart Home
- IoT
- Health
- Hardware
---
