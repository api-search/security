---
api_specs:
- filename: siebly-openapi-generated.yml
  format: yaml
  label: Siebly API
  slug: siebly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/siebly/openapi/_ae-authored/siebly-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: siebly.io
  spf: true
hosts:
- cert_expires: Dec 21 14:20:24 2026 GMT
  host: siebly.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Siebly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siebly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Siebly
provider_slug: siebly
slug: siebly-domain-security
source_filename: siebly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siebly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 14:20:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: siebly.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/siebly/security/siebly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SDK
- Cryptocurrency
- JavaScript
- TypeScript
- Exchange
---
