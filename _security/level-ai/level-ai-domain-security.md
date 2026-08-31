---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thelevel.ai
  spf: true
hosts:
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: thelevel.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Level Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Level AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Level AI
provider_slug: level-ai
slug: level-ai-domain-security
source_filename: level-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thelevel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thelevel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level-ai/refs/heads/main/security/level-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Contact Center
- Customer Experience
- Conversational Intelligence
- Auto QA
- Quality Assurance
- Agent Assist
- Voice Of The Customer
- Generative AI
- Voice AI
- Speech Recognition
- Sentiment Analysis
- Coaching
- Call Center Analytics
- LLM
---
