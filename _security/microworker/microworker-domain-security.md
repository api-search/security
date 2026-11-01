---
api_specs:
- filename: microworker-v1-openapi.json
  format: json
  label: Microworker API V1 API
  slug: microworker-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microworker/openapi/_original/microworker-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: microworker.app
  spf: true
hosts:
- cert_expires: Jan 11 15:21:21 2027 GMT
  host: microworker.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Microworker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microworker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microworker
provider_slug: microworker
slug: microworker-domain-security
source_filename: microworker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microworker.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 15:21:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microworker.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/microworker/security/microworker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Data Entry
- Testing
- Surveys
- Social Media Engagement
---
