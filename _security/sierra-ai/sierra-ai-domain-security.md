---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sierra.ai
  spf: true
hosts:
- cert_expires: Sep 18 02:57:02 2026 GMT
  host: sierra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sierra Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sierra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sierra
provider_slug: sierra-ai
slug: sierra-ai-domain-security
source_filename: sierra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sierra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:57:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sierra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sierra-ai/refs/heads/main/security/sierra-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Conversational AI
- Customer Experience
- Customer Service
- Agents
- AI Agents
- Voice
- Contact Center
- Enterprise
- Outcome-Based Pricing
- Agent OS
- Agent SDK
- Ghostwriter
- Bret Taylor
---
