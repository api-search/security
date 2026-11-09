---
api_specs:
- filename: decknote-app-openapi-generated.yml
  format: yaml
  label: decknote-app API
  slug: decknote-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decknote-app/openapi/_ae-authored/decknote-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: decknote.app
  spf: false
hosts:
- cert_expires: Dec  4 22:52:56 2026 GMT
  host: decknote.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Decknote App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for decknote-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: decknote-app
provider_slug: decknote-app
slug: decknote-app-domain-security
source_filename: decknote-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decknote.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 22:52:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: decknote.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/decknote-app/security/decknote-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Kanban
- Collaboration
- REST API
- PWA
- Automation
---
