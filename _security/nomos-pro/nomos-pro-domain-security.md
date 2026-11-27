---
api_specs:
- filename: nomos-pro-search-api-openapi.yml
  format: yaml
  label: Nomos Search API
  slug: nomos-pro-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomos-pro/openapi/nomos-pro-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nomos.pro
  spf: false
hosts:
- cert_expires: Jan  8 14:58:59 2027 GMT
  host: nomos.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nomos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Nomos
provider_slug: nomos-pro
slug: nomos-pro-domain-security
source_filename: nomos-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomos.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:58:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nomos.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nomos-pro/security/nomos-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Regulatory
- Compliance
- Monitoring
- Legislative
---
