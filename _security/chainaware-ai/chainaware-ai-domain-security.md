---
api_specs:
- filename: chainaware-ai-enterprise-api-openapi.yml
  format: yaml
  label: ChainAware Enterprise API
  slug: chainaware-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/openapi/chainaware-ai-enterprise-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: chainaware.ai
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: chainaware.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: enterprise.api.chainaware.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: prediction.mcp.chainaware.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Chainaware Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChainAware.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ChainAware.ai
provider_slug: chainaware-ai
slug: chainaware-ai-domain-security
source_filename: chainaware-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chainaware.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: enterprise.api.chainaware.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\n- host: prediction.mcp.chainaware.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chainaware.ai\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/security/chainaware-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- DeFi
- Fraud Detection
- AML
- Compliance
- Credit Scoring
- Risk Scoring
- Smart Contract Security
- Agent Trust
- MCP
- A2A
- x402
- Agents
- agent-native
- Estonia
---
