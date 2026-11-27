---
api_specs:
- filename: flitlink-com-openapi.yml
  format: yaml
  label: Flit API
  slug: flit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flitlink-com/openapi/flitlink-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flitlink.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: flitlink.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Flit
provider_slug: flitlink-com
slug: flitlink-com-domain-security
source_filename: flitlink-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flitlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: flitlink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flitlink-com/security/flitlink-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- URL Shortening
- QR Codes
- Analytics
---
