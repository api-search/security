---
api_specs:
- filename: myagi-bot-contact-api-openapi.yml
  format: yaml
  label: Myagi Contact API
  slug: myagi-bot-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-contact-api-openapi.yml
- filename: myagi-bot-mcp-api-openapi.yml
  format: yaml
  label: Myagi MCP API
  slug: myagi-bot-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-mcp-api-openapi.yml
- filename: myagi-bot-well-known-api-openapi.yml
  format: yaml
  label: Myagi .well Known API
  slug: myagi-bot-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myagi-bot/openapi/myagi-bot-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myagi.bot
  spf: true
hosts:
- cert_expires: Jan  6 01:57:29 2027 GMT
  host: myagi.bot
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Myagi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Myagi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Myagi
provider_slug: myagi-bot
slug: myagi-bot-domain-security
source_filename: myagi-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myagi.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 01:57:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myagi.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/myagi-bot/security/myagi-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Governance
- Cloud
- Governance
- Privacy
- Security
- Company
---
