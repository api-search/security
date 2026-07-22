---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gooddriver.ai
  spf: true
hosts:
- cert_expires: Sep  4 13:07:21 2026 GMT
  host: www.gooddriver.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Good Driver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Good Driver, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Good Driver
provider_slug: good-driver
slug: good-driver-domain-security
source_filename: good-driver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gooddriver.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:07:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gooddriver.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-driver/refs/heads/main/security/good-driver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Auto Insurance
- Financial Services
- Mobile App
- Consumer
- Vehicle Coverage
---
