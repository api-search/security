---
api_specs:
- filename: inbin-dev-openapi-generated.yml
  format: yaml
  label: Inbin API
  slug: inbin-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inbin-dev/openapi/_ae-authored/inbin-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inbin.dev
  spf: true
hosts:
- cert_expires: Dec 24 17:43:06 2026 GMT
  host: inbin.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inbin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inbin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inbin
provider_slug: inbin-dev
slug: inbin-dev-domain-security
source_filename: inbin-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inbin.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 17:43:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inbin.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inbin-dev/security/inbin-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Email API
- AI Integration
- Security
- Software-as-a-Service
---
