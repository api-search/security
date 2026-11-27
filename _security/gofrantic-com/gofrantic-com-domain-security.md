---
api_specs:
- filename: gofrantic-com-api-openapi.json
  format: json
  label: Frantic public API API
  slug: frantic-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gofrantic-com/openapi/_original/gofrantic-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gofrantic.com
  spf: false
hosts:
- cert_expires: Jan  6 08:15:11 2027 GMT
  host: gofrantic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frantic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frantic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Frantic
provider_slug: gofrantic-com
slug: gofrantic-com-domain-security
source_filename: gofrantic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gofrantic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 08:15:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gofrantic.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gofrantic-com/security/gofrantic-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Bounty
- Marketplace
- Payments
- OpenLedger
---
