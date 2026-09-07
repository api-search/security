---
api_specs:
- filename: openapi.json
  format: json
  label: Cracked API
  slug: cracked-api
  spec_type: OpenAPI
  url: https://cracked.ai/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cracked.ai
  spf: true
hosts:
- cert_expires: Dec  1 17:17:35 2026 GMT
  host: cracked.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cracked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cracked API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cracked API
provider_slug: cracked
slug: cracked-domain-security
source_filename: cracked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cracked.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 17:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cracked.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/security/cracked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ai agents
- agent tools
- mcp
- tool router
- API aggregator
- web search
- web scraping
- data enrichment
- llms.txt
- agent skills
- pay-per-call
- ai-agents
- agent-tools
- tool-router
- aggregator
- web-search
- web-scraping
- data-enrichment
- lead-generation
- ai-models
- developer-tools
- AI agents
- MCP
- lead gen
- SEO
- social media data
- ecommerce
- finance
- weather
- AI models
---
