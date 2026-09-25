---
api_specs:
- filename: berrergate-com-openapi.json
  format: json
  label: BerrerGate Tool & Provider Intelligence API
  slug: berrergate-tool-provider-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/berrergate-com/refs/heads/main/openapi/berrergate-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: berrergate.com
  spf: false
hosts:
- cert_expires: Nov 26 15:04:50 2026 GMT
  host: berrergate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Berrergate Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Berrer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Berrer
provider_slug: berrergate-com
slug: berrergate-com-domain-security
source_filename: berrergate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: berrergate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 15:04:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: berrergate.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/berrergate-com/refs/heads/main/security/berrergate-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Procurement
- Tool Discovery
- API Discovery
- AI Inference
- Research
- Agent-Native
---
