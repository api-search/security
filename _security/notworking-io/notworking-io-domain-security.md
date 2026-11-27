---
api_specs:
- filename: notworking-io-agents-api-openapi.yml
  format: yaml
  label: NotWorking Agents API
  slug: notworking-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notworking-io/openapi/notworking-io-agents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: notworking.io
  spf: false
hosts:
- cert_expires: Jan  7 01:27:45 2027 GMT
  host: notworking.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NotWorking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NotWorking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NotWorking
provider_slug: notworking-io
slug: notworking-io-domain-security
source_filename: notworking-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notworking.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 01:27:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: notworking.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/notworking-io/security/notworking-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- downdetector
- AI Agents
- MCP
- Plugins
---
