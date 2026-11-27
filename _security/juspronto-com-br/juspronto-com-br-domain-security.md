---
api_specs:
- filename: juspronto-com-br-mcp-api-openapi.yml
  format: yaml
  label: JusPronto MCP API
  slug: juspronto-com-br-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juspronto-com-br/openapi/juspronto-com-br-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: juspronto.com.br
  spf: true
hosts:
- cert_expires: Jan 21 03:02:34 2027 GMT
  host: juspronto.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JusPronto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JusPronto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JusPronto
provider_slug: juspronto-com-br
slug: juspronto-com-br-domain-security
source_filename: juspronto-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juspronto.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 03:02:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: juspronto.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/juspronto-com-br/security/juspronto-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Artificial Intelligence
- Software
- Brazil
- Software-as-a-Service
---
