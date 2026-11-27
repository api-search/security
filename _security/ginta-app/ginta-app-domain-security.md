---
api_specs:
- filename: ginta-app-openapi-generated.yml
  format: yaml
  label: Ginta API
  slug: ginta-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ginta-app/openapi/_ae-authored/ginta-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ginta.app
  spf: true
hosts:
- cert_expires: Jan  9 13:26:13 2027 GMT
  host: ginta.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ginta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ginta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ginta
provider_slug: ginta-app
slug: ginta-app-domain-security
source_filename: ginta-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ginta.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 13:26:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ginta.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ginta-app/security/ginta-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Website Builder
- Small Business
- No-Code
- Automation
---
