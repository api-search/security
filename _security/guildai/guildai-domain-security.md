---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: guild.ai
  spf: true
hosts:
- cert_expires: Oct 12 21:08:41 2026 GMT
  host: www.guild.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guildai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guild.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Guild.ai
provider_slug: guildai
slug: guildai-domain-security
source_filename: guildai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guild.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: guild.ai\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guildai/refs/heads/main/security/guildai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- AI Agents
- Agent Control Plane
- Agent Runtime
- Developer Tools
- MCP
- LLM
- Agent Governance
- SDK
- CLI
---
