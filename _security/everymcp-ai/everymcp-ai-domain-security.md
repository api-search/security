---
api_specs:
- filename: everymcp-ai-openapi-generated.yml
  format: yaml
  label: Every MCP API
  slug: everymcp-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everymcp-ai/openapi/_ae-authored/everymcp-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: everymcp.ai
  spf: true
hosts:
- cert_expires: Jan  5 00:27:41 2027 GMT
  host: everymcp.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Every MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Every MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Every MCP
provider_slug: everymcp-ai
slug: everymcp-ai-domain-security
source_filename: everymcp-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everymcp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:27:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: everymcp.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/everymcp-ai/security/everymcp-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- MCP
- Automation
- Productivity
- Integration
---
