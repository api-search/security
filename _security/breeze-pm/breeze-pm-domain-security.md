---
api_specs:
- filename: breeze-pm-openapi-generated.yml
  format: yaml
  label: breeze-pm API
  slug: breeze-pm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breeze-pm/openapi/_ae-authored/breeze-pm-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: breeze.pm
  spf: true
hosts:
- cert_expires: Dec 11 23:09:29 2026 GMT
  host: breeze.pm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: breeze-pm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for breeze-pm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: breeze-pm
provider_slug: breeze-pm
slug: breeze-pm-domain-security
source_filename: breeze-pm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breeze.pm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:09:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: breeze.pm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/breeze-pm/security/breeze-pm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Task Management
- Time Tracking
- Kanban
- Remote Work
---
