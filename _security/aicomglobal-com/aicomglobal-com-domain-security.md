---
api_specs:
- filename: aicomglobal-com-openapi.json
  format: json
  label: aicomglobal API
  slug: aicomglobal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aicomglobal.com
  spf: false
hosts:
- cert_expires: Nov 14 00:40:18 2026 GMT
  host: aicomglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aicomglobal Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aicomglobal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: aicomglobal
provider_slug: aicomglobal-com
slug: aicomglobal-com-domain-security
source_filename: aicomglobal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicomglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 00:40:18 2026 GMT\n  hsts: false\ndomains:\n- domain: aicomglobal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/security/aicomglobal-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Trust
- Reliability Monitoring
- Agent Discovery
- Agent Messaging
- Developer Tools
- Agent-Native
- United Kingdom
---
