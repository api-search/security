---
api_specs:
- filename: poof-bg-account-api-openapi.yml
  format: yaml
  label: poof-bg Account API
  slug: poof-bg-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/poof-bg/openapi/poof-bg-account-api-openapi.yml
- filename: poof-bg-background-removal-api-openapi.yml
  format: yaml
  label: poof-bg Background Removal API
  slug: poof-bg-background-removal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/poof-bg/openapi/poof-bg-background-removal-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: poof.bg
  spf: true
hosts:
- cert_expires: Dec 25 20:44:22 2026 GMT
  host: poof.bg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 12:18:28 2026 GMT
  host: api.poof.bg
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Poof Bg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for poof-bg, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: poof-bg
provider_slug: poof-bg
slug: poof-bg-domain-security
source_filename: poof-bg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poof.bg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 20:44:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.poof.bg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:18:28 2026 GMT\n  hsts: null\ndomains:\n- domain: poof.bg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/poof-bg/security/poof-bg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- BackgroundRemoval
- ImageProcessing
- VideoProcessing
---
