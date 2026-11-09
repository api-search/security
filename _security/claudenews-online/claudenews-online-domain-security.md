---
api_specs:
- filename: claudenews-online-openapi-generated.yml
  format: yaml
  label: Claude News API
  slug: claudenews-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claudenews-online/openapi/_ae-authored/claudenews-online-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: claudenews.online
  spf: false
hosts:
- cert_expires: Jan 17 13:40:23 2027 GMT
  host: claudenews.online
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claudenews Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claude News, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Claude News
provider_slug: claudenews-online
slug: claudenews-online-domain-security
source_filename: claudenews-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claudenews.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 13:40:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: claudenews.online\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/claudenews-online/security/claudenews-online-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- News
- Artificial Intelligence
- Anthropic
- Real-Time
- Aggregator
---
