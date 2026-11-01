---
api_specs:
- filename: heard-dev-openapi-generated.yml
  format: yaml
  label: heard-dev API
  slug: heard-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heard-dev/openapi/_ae-authored/heard-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heard.dev
  spf: true
hosts:
- cert_expires: Jan 24 22:22:30 2027 GMT
  host: heard.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heard Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for heard-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: heard-dev
provider_slug: heard-dev
slug: heard-dev-domain-security
source_filename: heard-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heard.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 22:22:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: heard.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heard-dev/security/heard-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Voice
- macOS
- DeveloperTools
---
