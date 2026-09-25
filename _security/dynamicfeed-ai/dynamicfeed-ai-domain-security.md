---
api_specs:
- filename: dynamicfeed-ai-openapi.yml
  format: yaml
  label: Dynamic Feed REST API
  slug: dynamic-feed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamicfeed-ai/refs/heads/main/openapi/dynamicfeed-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dynamicfeed.ai
  spf: true
hosts:
- cert_expires: Oct 25 22:51:46 2026 GMT
  host: dynamicfeed.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynamicfeed Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic Feed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dynamic Feed
provider_slug: dynamicfeed-ai
slug: dynamicfeed-ai-domain-security
source_filename: dynamicfeed-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynamicfeed.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 22:51:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dynamicfeed.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamicfeed-ai/refs/heads/main/security/dynamicfeed-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Live Data
- AI Agents
- MCP
- A2A
- Agent-Native
- Provenance
- Weather
- Natural Hazards
- Vulnerabilities
- Sanctions
- Space
- Robotics
- x402
- Receipts
- Notary
- Australia
---
