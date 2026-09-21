---
api_specs:
- filename: fodda-ai-openapi.yml
  format: yaml
  label: Fodda Context & Research API
  slug: fodda-context-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/openapi/fodda-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fodda.ai
  spf: false
hosts:
- cert_expires: Nov 25 22:07:14 2026 GMT
  host: fodda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 02:15:45 2026 GMT
  host: www.fodda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 19:18:40 2026 GMT
  host: api.fodda.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fodda Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fodda (PSFK), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Fodda (PSFK)
provider_slug: fodda-ai
slug: fodda-ai-domain-security
source_filename: fodda-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fodda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 22:07:14 2026 GMT\n  hsts: false\n- host: www.fodda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 02:15:45 2026 GMT\n  hsts: false\n- host: api.fodda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 19:18:40 2026 GMT\n  hsts: null\ndomains:\n- domain: fodda.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/security/fodda-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Market Intelligence
- Trend Research
- Knowledge Graph
- Consumer Insights
- Earnings Intelligence
- Brand Intelligence
- Research
- Institutional Data
- MCP
- A2A
- agent-native
- Machine Payments
- Company
---
