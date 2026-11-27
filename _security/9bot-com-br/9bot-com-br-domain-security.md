---
api_specs:
- filename: 9bot-com-br-discovery-api-openapi.yml
  format: yaml
  label: 9bot Discovery API
  slug: 9bot-com-br-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-discovery-api-openapi.yml
- filename: 9bot-com-br-health-api-openapi.yml
  format: yaml
  label: 9bot Health API
  slug: 9bot-com-br-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-health-api-openapi.yml
- filename: 9bot-com-br-mcp-api-openapi.yml
  format: yaml
  label: 9bot MCP API
  slug: 9bot-com-br-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 9bot.com.br
  spf: true
hosts:
- cert_expires: Dec  8 17:02:59 2026 GMT
  host: 9bot.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 9bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 9bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 9bot
provider_slug: 9bot-com-br
slug: 9bot-com-br-domain-security
source_filename: 9bot-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 9bot.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 17:02:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 9bot.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/9bot-com-br/security/9bot-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WhatsApp
- Automation
- Bot
- Messaging
- Integration
---
