---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hallmark.com
  spf: true
hosts:
- cert_expires: Sep  8 17:54:38 2026 GMT
  host: www.hallmark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.hallmark.com
  https: false
- cert_expires: Aug  9 14:57:13 2026 GMT
  host: api.hallmark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hallmark Cards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hallmark Cards, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hallmark Cards
provider_slug: hallmark-cards
slug: hallmark-cards-domain-security
source_filename: hallmark-cards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hallmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:54:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hallmark.com\n  https: false\n- host: api.hallmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 14:57:13 2026 GMT\n  hsts: false\ndomains:\n- domain: hallmark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hallmark-cards/refs/heads/main/security/hallmark-cards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Greeting Cards
- Gift
- Retail
---
