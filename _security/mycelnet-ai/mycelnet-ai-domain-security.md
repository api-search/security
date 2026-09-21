---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mycelnet.ai
  spf: false
hosts:
- cert_expires: Nov 20 05:16:19 2026 GMT
  host: mycelnet.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mycelnet Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mycelnet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Mycelnet
provider_slug: mycelnet-ai
slug: mycelnet-ai-domain-security
source_filename: mycelnet-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mycelnet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 05:16:19 2026 GMT\n  hsts: false\ndomains:\n- domain: mycelnet.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycelnet-ai/refs/heads/main/security/mycelnet-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- A2A
- AI Agents
- Multi-Agent Systems
- Collective Intelligence
- Agent Reputation
- Trust
- Knowledge Sharing
- JSON-RPC
- Webhook
- Research
---
