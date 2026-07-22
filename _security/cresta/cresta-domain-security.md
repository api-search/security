---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cresta.com
  spf: true
hosts:
- cert_expires: Aug 11 21:43:07 2026 GMT
  host: cresta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cresta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cresta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cresta
provider_slug: cresta
slug: cresta-domain-security
source_filename: cresta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cresta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 21:43:07 2026 GMT\n  hsts: false\ndomains:\n- domain: cresta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cresta/refs/heads/main/security/cresta-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Artificial Intelligence
- Contact Center
- Contact Center AI
- CCaaS
- Customer Experience
- Conversational AI
- Voice AI
- Agent Assist
- Conversation Intelligence
- Knowledge Agent
- Quality Management
- Real-Time Coaching
- After-Call Automation
- Enterprise AI
- MCP
---
