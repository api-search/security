---
api_specs:
- filename: 9992507-1975dcee-1898-4584-8046-2deae6997e7a
  format: yaml
  label: 360VUZ Creator API
  slug: 360vuz-creator-api
  spec_type: Postman
  url: https://vuz360.postman.co/collections/9992507-1975dcee-1898-4584-8046-2deae6997e7a?version=latest&workspace=3e546806-ec08-487d-ad9c-99bd8ee0c9c6
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vuz.com
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: vuz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 360 Vuz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 360 VUZ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 360 VUZ
provider_slug: 360-vuz
slug: 360-vuz-domain-security
source_filename: 360-vuz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vuz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vuz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/360-vuz/refs/heads/main/security/360-vuz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Streaming
- Virtual Reality
- Immersive Media
- 360 Video
- Entertainment
- Media
---
