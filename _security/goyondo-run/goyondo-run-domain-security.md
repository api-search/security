---
api_specs:
- filename: goyondo-run-api-openapi.json
  format: json
  label: Goyondo API API
  slug: goyondo-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goyondo-run/openapi/_original/goyondo-run-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goyondo.run
  spf: false
hosts:
- cert_expires: Dec 24 21:32:26 2026 GMT
  host: goyondo.run
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goyondo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goyondo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Goyondo
provider_slug: goyondo-run
slug: goyondo-run-domain-security
source_filename: goyondo-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goyondo.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 21:32:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goyondo.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goyondo-run/security/goyondo-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Artificial Intelligence
- Trip Planning
- Group Travel
---
