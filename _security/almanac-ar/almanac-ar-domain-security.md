---
api_specs:
- filename: almanac-ar-v1-openapi.json
  format: json
  label: Almanac API V1 API
  slug: almanac-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/almanac-ar/openapi/_original/almanac-ar-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: almanac.ar
  spf: true
hosts:
- cert_expires: Dec  4 16:20:00 2026 GMT
  host: almanac.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Almanac Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Almanac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Almanac
provider_slug: almanac-ar
slug: almanac-ar-domain-security
source_filename: almanac-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: almanac.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 16:20:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: almanac.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/almanac-ar/security/almanac-ar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
