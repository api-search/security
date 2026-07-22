---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itsgood.life
  spf: true
hosts:
- cert_expires: Oct 16 00:17:59 2026 GMT
  host: itsgood.life
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Its Good Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Its Good, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Its Good
provider_slug: its-good
slug: its-good-domain-security
source_filename: its-good-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itsgood.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:17:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: itsgood.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/its-good/refs/heads/main/security/its-good-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurants
- Dining
- Recommendations
- Social
- Food and Drink
- Consumer
- Mobile
- Discovery
---
