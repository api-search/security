---
api_specs:
- filename: firmoscop-ro-api-openapi.json
  format: json
  label: Firmoscop API API
  slug: firmoscop-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmoscop-ro/openapi/_original/firmoscop-ro-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firmoscop.ro
  spf: true
hosts:
- cert_expires: Feb  5 16:43:48 2027 GMT
  host: firmoscop.ro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmoscop Ro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firmoscop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Firmoscop
provider_slug: firmoscop-ro
slug: firmoscop-ro-domain-security
source_filename: firmoscop-ro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firmoscop.ro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 16:43:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firmoscop.ro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firmoscop-ro/security/firmoscop-ro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Data
- API
- Romania
- Business
---
