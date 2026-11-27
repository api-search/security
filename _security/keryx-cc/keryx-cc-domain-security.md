---
api_specs:
- filename: keryx-cc-openapi-generated.yml
  format: yaml
  label: Keryx API
  slug: keryx-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keryx-cc/openapi/_ae-authored/keryx-cc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keryx.cc
  spf: true
hosts:
- cert_expires: Jan 10 02:57:50 2027 GMT
  host: keryx.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keryx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keryx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Keryx
provider_slug: keryx-cc
slug: keryx-cc-domain-security
source_filename: keryx-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keryx.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 02:57:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: keryx.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/keryx-cc/security/keryx-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Research
- Platform
- Open Source
- Blockchain
---
