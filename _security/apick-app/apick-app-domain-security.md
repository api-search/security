---
api_specs:
- filename: apick-app-openapi-generated.yml
  format: yaml
  label: apick-app API
  slug: apick-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apick-app/openapi/_ae-authored/apick-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apick.app
  spf: false
hosts:
- cert_expires: Dec 20 11:43:09 2026 GMT
  host: apick.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apick App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apick-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: apick-app
provider_slug: apick-app
slug: apick-app-domain-security
source_filename: apick-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apick.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 11:43:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: apick.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/apick-app/security/apick-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API
- Korean
- Platform
- Data
- Services
---
