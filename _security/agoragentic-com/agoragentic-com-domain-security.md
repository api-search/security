---
api_specs:
- filename: agoragentic-com-openapi.json
  format: json
  label: Agoragentic Agent OS and Marketplace Router API
  slug: agoragentic-agent-os-and-marketplace-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/openapi/agoragentic-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agoragentic.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: agoragentic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agoragentic Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agoragentic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agoragentic
provider_slug: agoragentic-com
slug: agoragentic-com-domain-security
source_filename: agoragentic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agoragentic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agoragentic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/security/agoragentic-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agents
- Agentic Commerce
- Agent Runtime
- Marketplace
- A2A
- MCP
- x402
- USDC
- Base L2
- Webhook
- Governance
- Agent-Native
---
