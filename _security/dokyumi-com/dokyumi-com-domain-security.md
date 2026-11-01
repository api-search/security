---
api_specs:
- filename: dokyumi-com-openapi-generated.yml
  format: yaml
  label: dokyumi-com API
  slug: dokyumi-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dokyumi-com/openapi/_ae-authored/dokyumi-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dokyumi.com
  spf: true
hosts:
- cert_expires: Jan  4 22:14:11 2027 GMT
  host: dokyumi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dokyumi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dokyumi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dokyumi-com
provider_slug: dokyumi-com
slug: dokyumi-com-domain-security
source_filename: dokyumi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dokyumi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:14:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dokyumi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dokyumi-com/security/dokyumi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document-Parsing
- API
- OCR
- SaaS
- Finance
---
