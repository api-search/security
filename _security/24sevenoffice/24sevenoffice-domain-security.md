---
api_specs:
- filename: 24sevenoffice-openapi-generated.yml
  format: yaml
  label: Finago API
  slug: 24sevenoffice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/24sevenoffice/openapi/_ae-authored/24sevenoffice-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: finago.no
  spf: true
hosts:
- cert_expires: Jan 31 05:45:42 2027 GMT
  host: finago.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Finago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finago, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Finago
provider_slug: 24sevenoffice
slug: 24sevenoffice-domain-security
source_filename: 24sevenoffice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finago.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 05:45:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finago.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/24sevenoffice/security/24sevenoffice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Payroll
- Business Management
- Norway
- Sweden
- Finland
---
