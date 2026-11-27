---
api_specs:
- filename: fairly-gg-api-openapi.json
  format: json
  label: Fairly API API
  slug: fairly-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairly-gg/openapi/_original/fairly-gg-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fairly.gg
  spf: false
hosts:
- cert_expires: Jan  7 11:10:32 2027 GMT
  host: fairly.gg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fairly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fairly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fairly
provider_slug: fairly-gg
slug: fairly-gg-domain-security
source_filename: fairly-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fairly.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 11:10:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fairly.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fairly-gg/security/fairly-gg-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Gaming
- Price Comparison
- Open Data
- Fair Pricing
---
