---
api_specs:
- filename: e18e-dev-openapi-generated.yml
  format: yaml
  label: e18e API
  slug: e18e-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e18e-dev/openapi/_ae-authored/e18e-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: e18e.dev
  spf: false
hosts:
- cert_expires: Feb  2 15:54:36 2027 GMT
  host: e18e.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: E18E Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for e18e, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: e18e
provider_slug: e18e-dev
slug: e18e-dev-domain-security
source_filename: e18e-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: e18e.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 15:54:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: e18e.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/e18e-dev/security/e18e-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Ecosystem
- Performance
- JavaScript
- Open Source
- Community
---
