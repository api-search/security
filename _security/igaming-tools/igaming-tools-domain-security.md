---
api_specs:
- filename: igaming-tools-openapi.json
  format: json
  label: iGamingScraper REST API
  slug: igamingscraper-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igaming-tools/refs/heads/main/openapi/igaming-tools-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: i-gaming.tools
  spf: true
hosts:
- cert_expires: Oct 13 07:35:10 2026 GMT
  host: i-gaming.tools
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 07:35:10 2026 GMT
  host: mcp.i-gaming.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Igaming Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iGaming Tools, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iGaming Tools
provider_slug: igaming-tools
slug: igaming-tools-domain-security
source_filename: igaming-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: i-gaming.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:35:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.i-gaming.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:35:10 2026 GMT\n  hsts: false\ndomains:\n- domain: i-gaming.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igaming-tools/refs/heads/main/security/igaming-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- iGaming
- Online Casino
- Gambling
- slot games
- slot metadata
- gambling regulation
- Industry News
- Job
- market demand
- Analytics
- REST API
- OpenAPI
- MCP Server
- llms-txt
- LLM Tooling
- slot RTP
- paytable data
- search demand
- iGaming jobs
- agent-ready API
- read-only API
---
