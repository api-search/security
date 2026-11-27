---
api_specs:
- filename: oaia-fun-openapi-generated.yml
  format: yaml
  label: OAIA API
  slug: oaia-fun-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oaia-fun/openapi/_ae-authored/oaia-fun-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oaia.fun
  spf: false
hosts:
- cert_expires: Jan 17 14:20:34 2027 GMT
  host: oaia.fun
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OAIA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OAIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OAIA
provider_slug: oaia-fun
slug: oaia-fun-domain-security
source_filename: oaia-fun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oaia.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 14:20:34 2027 GMT\n  hsts: false\ndomains:\n- domain: oaia.fun\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/oaia-fun/security/oaia-fun-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Trading
- Benchmarks
- Finance
- Open Source
---
