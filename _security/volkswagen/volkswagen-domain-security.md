---
api_specs:
- filename: volkswagen-okapi-openapi.yml
  format: yaml
  label: Volkswagen OKAPI - Open Konfigurator API
  slug: volkswagen-okapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volkswagen/refs/heads/main/openapi/volkswagen-okapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: volkswagenag.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: okapi-ddp.productdata.volkswagenag.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: productdata.volkswagenag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volkswagen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volkswagen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Volkswagen
provider_slug: volkswagen
slug: volkswagen-domain-security
source_filename: volkswagen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: okapi-ddp.productdata.volkswagenag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\n- host: productdata.volkswagenag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: volkswagenag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volkswagen/refs/heads/main/security/volkswagen-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automobiles
- Cars
- Vehicles
- Automotive
- Vehicle Configuration
---
