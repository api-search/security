---
api_specs:
- filename: hatchable-site-openapi.yml
  format: yaml
  label: IntentGuard Router API
  slug: intentguard-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hatchable-site/refs/heads/main/openapi/hatchable-site-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hatchable.site
  spf: false
hosts:
- cert_expires: Dec 18 15:43:16 2026 GMT
  host: intentguard.hatchable.site
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hatchable Site Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IntentGuard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: IntentGuard
provider_slug: hatchable-site
slug: hatchable-site-domain-security
source_filename: hatchable-site-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intentguard.hatchable.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 15:43:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hatchable.site\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hatchable-site/refs/heads/main/security/hatchable-site-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Model Routing
- Cost Optimization
- x402
- MCP
- A2A
- pay-per-call
- Prompt Optimization
- Agent Payments
---
