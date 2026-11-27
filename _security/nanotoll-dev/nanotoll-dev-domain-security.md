---
api_specs:
- filename: nanotoll-dev-account-api-openapi.yml
  format: yaml
  label: Nanotoll Account API
  slug: nanotoll-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanotoll-dev/openapi/nanotoll-dev-account-api-openapi.yml
- filename: nanotoll-dev-operational-api-openapi.yml
  format: yaml
  label: Nanotoll Operational API
  slug: nanotoll-dev-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanotoll-dev/openapi/nanotoll-dev-operational-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nanotoll.dev
  spf: true
hosts:
- cert_expires: Jan 24 21:23:02 2027 GMT
  host: nanotoll.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nanotoll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanotoll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nanotoll
provider_slug: nanotoll-dev
slug: nanotoll-dev-domain-security
source_filename: nanotoll-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanotoll.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 21:23:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nanotoll.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nanotoll-dev/security/nanotoll-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM
- Compression
- USDC
- Base
---
