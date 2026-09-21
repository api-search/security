---
api_specs:
- filename: iwant-fyi-openapi.yml
  format: yaml
  label: iwant.fyi Agent API
  slug: iwantfyi-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iwant-fyi/refs/heads/main/openapi/iwant-fyi-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iwant.fyi
  spf: true
hosts:
- cert_expires: Nov  4 08:35:16 2026 GMT
  host: iwant.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iwant Fyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iwant.fyi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iwant.fyi
provider_slug: iwant-fyi
slug: iwant-fyi-domain-security
source_filename: iwant-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iwant.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 08:35:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: iwant.fyi\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iwant-fyi/refs/heads/main/security/iwant-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic Commerce
- Marketplace
- AI Agents
- Purchase Intent
- Shopping
- Automotive
- MCP
- A2A
- Open Protocol
- x402
- agent-native
---
