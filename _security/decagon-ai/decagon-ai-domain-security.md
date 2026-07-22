---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: decagon.ai
  spf: true
hosts:
- cert_expires: Aug 14 18:47:22 2026 GMT
  host: decagon.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decagon Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decagon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Decagon
provider_slug: decagon-ai
slug: decagon-ai-domain-security
source_filename: decagon-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decagon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 18:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: decagon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decagon-ai/refs/heads/main/security/decagon-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- AI Agents
- Customer Support
- Customer Experience
- Customer Service
- Contact Center
- Conversational AI
- Voice AI
- Chatbots
- Email
- SMS
- Model Context Protocol
- Enterprise
---
