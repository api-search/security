---
api_specs:
- filename: shoplazza-admin-openapi-original.json
  format: json
  label: Shoplazza Admin API
  slug: shoplazza-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-admin-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shoplazza.dev
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: myshoplaza.com
  spf: false
hosts:
- cert_expires: Oct  2 23:40:31 2026 GMT
  host: www.shoplazza.dev
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 07:12:27 2026 GMT
  host: developer.myshoplaza.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shoplazza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shoplazza, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Shoplazza
provider_slug: shoplazza
slug: shoplazza-domain-security
source_filename: shoplazza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shoplazza.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:40:31 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: developer.myshoplaza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 07:12:27 2026 GMT\n  hsts: null\ndomains:\n- domain: shoplazza.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: myshoplaza.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/security/shoplazza-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise
- E-Commerce
- Online Store
- Retail
- Payments
- Webhooks
- REST API
- Apps
- Developer Platform
---
