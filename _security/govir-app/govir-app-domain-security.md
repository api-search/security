---
api_specs:
- filename: govir-app-openapi-generated.yml
  format: yaml
  label: Govir API
  slug: govir-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govir-app/openapi/_ae-authored/govir-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: govir.app
  spf: true
hosts:
- cert_expires: Dec 29 12:58:18 2026 GMT
  host: govir.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Govir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Govir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Govir
provider_slug: govir-app
slug: govir-app-domain-security
source_filename: govir-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govir.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 12:58:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govir.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/govir-app/security/govir-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Threads
- Scheduling
- AI writer
- Analytics
- Agency Tools
- Multi-Account
---
