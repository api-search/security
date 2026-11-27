---
api_specs:
- filename: eltablero-ar-openapi-generated.yml
  format: yaml
  label: El Tablero API
  slug: eltablero-ar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eltablero-ar/openapi/_ae-authored/eltablero-ar-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: eltablero.ar
  spf: true
hosts:
- cert_expires: Jan 12 11:20:24 2027 GMT
  host: eltablero.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: El Tablero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for El Tablero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: El Tablero
provider_slug: eltablero-ar
slug: eltablero-ar-domain-security
source_filename: eltablero-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eltablero.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 11:20:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eltablero.ar\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/eltablero-ar/security/eltablero-ar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
