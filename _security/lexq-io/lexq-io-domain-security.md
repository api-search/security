---
api_specs:
- filename: lexq-io-openapi-generated.yml
  format: yaml
  label: LexQ API
  slug: lexq-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexq-io/openapi/_ae-authored/lexq-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lexq.io
  spf: true
hosts:
- cert_expires: Dec 13 11:51:24 2026 GMT
  host: lexq.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LexQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LexQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LexQ
provider_slug: lexq-io
slug: lexq-io-domain-security
source_filename: lexq-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 11:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lexq.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lexq-io/security/lexq-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decision Operations
- Rule Engine
- Business Rules
- Audit Trail
- Impact Simulation
---
