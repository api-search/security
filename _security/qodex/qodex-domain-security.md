---
api_specs:
- filename: qodex-openapi-generated.yml
  format: yaml
  label: QodexAI API
  slug: qodex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qodex/openapi/_ae-authored/qodex-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qodex.ai
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: qodex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qodex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QodexAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QodexAI
provider_slug: qodex
slug: qodex-domain-security
source_filename: qodex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qodex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qodex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/qodex/security/qodex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Testing
- Continuous Integration
- DevOps
---
