---
api_specs:
- filename: smartcut-dev-openapi-openapi.json
  format: json
  label: SmartCut API V3 Openapi API
  slug: smartcut-api-v3-openapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smartcut-dev/openapi/_original/smartcut-dev-openapi-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smartcut.dev
  spf: false
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: smartcut.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smartcut Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for smartcut-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: smartcut-dev
provider_slug: smartcut-dev
slug: smartcut-dev-domain-security
source_filename: smartcut-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartcut.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smartcut.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/smartcut-dev/security/smartcut-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Developer Tools
- Automation
- CI/CD
- APIs
---
