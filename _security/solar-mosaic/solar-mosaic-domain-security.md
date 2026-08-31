---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinmosaic.com
  spf: true
hosts:
- cert_expires: Oct  5 19:59:51 2026 GMT
  host: joinmosaic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:43:29 2026 GMT
  host: developer.joinmosaic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.joinmosaic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solar Mosaic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solar Mosaic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Solar Mosaic
provider_slug: solar-mosaic
slug: solar-mosaic-domain-security
source_filename: solar-mosaic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinmosaic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:59:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.joinmosaic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:43:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.joinmosaic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: joinmosaic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solar-mosaic/refs/heads/main/security/solar-mosaic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Lending
- Solar
- Clean Energy
- Home Improvement Finance
- Point of Sale Financing
- Consumer Finance
- Defunct
---
