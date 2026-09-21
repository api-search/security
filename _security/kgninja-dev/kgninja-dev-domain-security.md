---
api_specs:
- filename: kgninja-dev-openapi.json
  format: json
  label: Agent Verification Utility API
  slug: agent-verification-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kgninja-dev/refs/heads/main/openapi/kgninja-dev-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kgninja.dev
  spf: true
hosts:
- cert_expires: Nov  6 03:05:24 2026 GMT
  host: agent-economy.kgninja.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kgninja Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KG-NINJA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: KG-NINJA
provider_slug: kgninja-dev
slug: kgninja-dev-domain-security
source_filename: kgninja-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-economy.kgninja.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 03:05:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kgninja.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kgninja-dev/refs/heads/main/security/kgninja-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Verification
- JSON
- Cryptography
- Cloudflare Workers
- agent-native
- Japan
---
