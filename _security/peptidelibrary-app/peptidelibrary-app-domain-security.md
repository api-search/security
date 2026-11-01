---
api_specs:
- filename: peptidelibrary-app-openapi-generated.yml
  format: yaml
  label: peptidelibrary-app API
  slug: peptidelibrary-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peptidelibrary-app/openapi/_ae-authored/peptidelibrary-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: peptidelibrary.app
  spf: true
hosts:
- cert_expires: Dec  6 15:24:42 2026 GMT
  host: peptidelibrary.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Peptidelibrary App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for peptidelibrary-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: peptidelibrary-app
provider_slug: peptidelibrary-app
slug: peptidelibrary-app-domain-security
source_filename: peptidelibrary-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peptidelibrary.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 15:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peptidelibrary.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/peptidelibrary-app/security/peptidelibrary-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Peptide Research
- Vendor Comparison
- Research Tools
- Inventory Management
---
