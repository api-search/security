---
api_specs:
- filename: aopx-fr-aopx-recommend-v0-api-openapi.yml
  format: yaml
  label: aopx-fr AOPX Recommend v0 API
  slug: aopx-fr-aopx-recommend-v0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aopx-fr/openapi/aopx-fr-aopx-recommend-v0-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aopx.fr
  spf: false
hosts:
- cert_expires: Jan 12 05:20:06 2027 GMT
  host: aopx.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aopx Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aopx-fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: aopx-fr
provider_slug: aopx-fr
slug: aopx-fr-domain-security
source_filename: aopx-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aopx.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 05:20:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aopx.fr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aopx-fr/security/aopx-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Search
- AI
- Routing
- Benchmark
- Evidence
---
