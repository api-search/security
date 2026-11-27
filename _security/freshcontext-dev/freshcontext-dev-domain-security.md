---
api_specs:
- filename: freshcontext-dev-openapi-generated.yml
  format: yaml
  label: FreshContext API
  slug: freshcontext-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freshcontext-dev/openapi/_ae-authored/freshcontext-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshcontext.dev
  spf: true
hosts:
- cert_expires: Jan  2 14:04:21 2027 GMT
  host: freshcontext.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FreshContext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreshContext, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FreshContext
provider_slug: freshcontext-dev
slug: freshcontext-dev-domain-security
source_filename: freshcontext-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freshcontext.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 14:04:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshcontext.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freshcontext-dev/security/freshcontext-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI workflow
- Context Integrity
- Integration
---
