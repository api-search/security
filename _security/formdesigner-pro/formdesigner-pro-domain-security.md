---
api_specs:
- filename: formdesigner-pro-openapi-generated.yml
  format: yaml
  label: FormDesigner API
  slug: formdesigner-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formdesigner-pro/openapi/_ae-authored/formdesigner-pro-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: formdesigner.pro
  spf: true
hosts:
- cert_expires: Dec 18 12:25:21 2026 GMT
  host: formdesigner.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FormDesigner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FormDesigner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FormDesigner
provider_slug: formdesigner-pro
slug: formdesigner-pro-domain-security
source_filename: formdesigner-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formdesigner.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:25:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: formdesigner.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/formdesigner-pro/security/formdesigner-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Form Builder
- Online Forms
- Quizzes
- Calculators
- Payments
- Integration
---
