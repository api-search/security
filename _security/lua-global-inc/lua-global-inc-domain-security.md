---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heylua.ai
  spf: true
hosts:
- cert_expires: Oct  5 16:21:53 2026 GMT
  host: heylua.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:21:53 2026 GMT
  host: docs.heylua.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:21:53 2026 GMT
  host: api.heylua.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lua Global Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lua Global Inc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lua Global Inc
provider_slug: lua-global-inc
slug: lua-global-inc-domain-security
source_filename: lua-global-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heylua.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:21:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.heylua.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:21:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.heylua.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:21:53 2026 GMT\n  hsts: null\ndomains:\n- domain: heylua.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lua-global-inc/refs/heads/main/security/lua-global-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Platform
- Developer Tools
- Model Context Protocol
- Conversational AI
- Chatbots
- Automation
---
