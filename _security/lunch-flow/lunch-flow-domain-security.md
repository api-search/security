---
api_specs:
- filename: lunch-flow-openapi-generated.yml
  format: yaml
  label: Lunch Flow API
  slug: lunch-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lunch-flow/openapi/_ae-authored/lunch-flow-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunchflow.app
  spf: false
hosts:
- cert_expires: Dec 29 18:43:39 2026 GMT
  host: www.lunchflow.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lunch Flow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunch Flow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lunch Flow
provider_slug: lunch-flow
slug: lunch-flow-domain-security
source_filename: lunch-flow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lunchflow.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 18:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lunchflow.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lunch-flow/security/lunch-flow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- API
- Banking
- Integration
- OpenAPI
- Developer
---
