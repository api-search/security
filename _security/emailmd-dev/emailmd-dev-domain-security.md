---
api_specs:
- filename: emailmd-dev-openapi-generated.yml
  format: yaml
  label: emailmd API
  slug: emailmd-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailmd-dev/openapi/_ae-authored/emailmd-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emailmd.dev
  spf: true
hosts:
- cert_expires: Dec 20 23:10:58 2026 GMT
  host: emailmd.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: emailmd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for emailmd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: emailmd
provider_slug: emailmd-dev
slug: emailmd-dev-domain-security
source_filename: emailmd-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailmd.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:10:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: emailmd.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/emailmd-dev/security/emailmd-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Markdown
- Templates
- Builder
---
