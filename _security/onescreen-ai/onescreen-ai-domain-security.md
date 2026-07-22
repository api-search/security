---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onescreen.ai
  spf: true
hosts:
- cert_expires: Sep  3 16:46:53 2026 GMT
  host: onescreen.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onescreen Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneScreen AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OneScreen AI
provider_slug: onescreen-ai
slug: onescreen-ai-domain-security
source_filename: onescreen-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onescreen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:46:53 2026 GMT\n  hsts: false\ndomains:\n- domain: onescreen.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onescreen-ai/refs/heads/main/security/onescreen-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Out-of-Home
- DOOH
- Advertising Technology
- Marketing
- Media
- AI Agents
- MCP
---
