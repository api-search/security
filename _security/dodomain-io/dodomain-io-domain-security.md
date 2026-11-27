---
api_specs:
- filename: dodomain-io-api-openapi.json
  format: json
  label: DoDomain API API
  slug: dodomain-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dodomain-io/openapi/_original/dodomain-io-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dodomain.io
  spf: true
hosts:
- cert_expires: Jan 25 23:59:49 2027 GMT
  host: dodomain.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DoDomain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoDomain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DoDomain
provider_slug: dodomain-io
slug: dodomain-io-domain-security
source_filename: dodomain-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dodomain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dodomain.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dodomain-io/security/dodomain-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- DNS
- CustomDomain
- Integration
---
