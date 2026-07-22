---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: context.ai
  spf: true
hosts:
- cert_expires: Sep  9 21:34:31 2026 GMT
  host: context.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contextai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Context.ai *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Context.ai *
provider_slug: contextai
slug: contextai-domain-security
source_filename: contextai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: context.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: context.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextai/refs/heads/main/security/contextai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Agents
- Enterprise AI
- Agent Platform
- LLM
- Automation
- Evaluation
---
