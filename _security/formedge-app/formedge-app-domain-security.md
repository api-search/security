---
api_specs:
- filename: formedge-app-openapi-generated.yml
  format: yaml
  label: Value Inc. API
  slug: formedge-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formedge-app/openapi/_ae-authored/formedge-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formedge.app
  spf: true
hosts:
- cert_expires: Jan 16 23:30:13 2027 GMT
  host: formedge.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Value Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Value Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Value Inc.
provider_slug: formedge-app
slug: formedge-app-domain-security
source_filename: formedge-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formedge.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:30:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: formedge.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/formedge-app/security/formedge-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- No-Code
- Form Builder
- Artificial Intelligence
- Japanese
---
