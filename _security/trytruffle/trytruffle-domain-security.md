---
api_specs:
- filename: trytruffle-agents-api-openapi.yml
  format: yaml
  label: Truffle AI Agents API
  slug: trytruffle-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trytruffle/openapi/trytruffle-agents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trytruffle.ai
  spf: true
hosts:
- cert_expires: Jan  9 13:06:56 2027 GMT
  host: trytruffle.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trytruffle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truffle AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truffle AI
provider_slug: trytruffle
slug: trytruffle-domain-security
source_filename: trytruffle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trytruffle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 13:06:56 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trytruffle.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/trytruffle/security/trytruffle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
