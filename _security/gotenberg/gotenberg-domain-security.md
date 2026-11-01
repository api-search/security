---
api_specs:
- filename: gotenberg-openapi-generated.yml
  format: yaml
  label: Gotenberg API
  slug: gotenberg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gotenberg/openapi/_ae-authored/gotenberg-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gotenberg.dev
  spf: true
hosts:
- cert_expires: Jan 19 17:10:22 2027 GMT
  host: gotenberg.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gotenberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gotenberg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Gotenberg
provider_slug: gotenberg
slug: gotenberg-domain-security
source_filename: gotenberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gotenberg.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 17:10:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: gotenberg.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gotenberg/security/gotenberg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- PDF
- Docker
- API
- Conversion
- OpenSource
---
