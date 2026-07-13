---
api_specs:
- filename: tesla-motors-owner-openapi.yml
  format: yaml
  label: Tesla Owner API
  slug: owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-motors/refs/heads/main/openapi/tesla-motors-owner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tesla.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: timdorr.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: developer.tesla.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.tesla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 19:47:10 2026 GMT
  host: tesla-api.timdorr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesla Motors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesla Motors, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tesla Motors
provider_slug: tesla-motors
slug: tesla-motors-domain-security
source_filename: tesla-motors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: tesla-api.timdorr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:47:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tesla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: timdorr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla-motors/refs/heads/main/security/tesla-motors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automobiles
- Electric Vehicles
- Cars
- Smart Vehicles
- IoT
- Fortune 1000
---
