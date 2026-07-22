---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: august.com
  spf: true
hosts:
- cert_expires: Aug 25 17:06:09 2026 GMT
  host: august.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: August Home Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for August Home, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: August Home
provider_slug: august-home
slug: august-home-domain-security
source_filename: august-home-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: august.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:06:09 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: august.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/august-home/refs/heads/main/security/august-home-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Smart Home
- Smart Lock
- Access Control
- Home Security
- IoT
- Consumer Electronics
- Yale
- ASSA ABLOY
---
