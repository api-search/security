---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: champ.ai
  spf: true
hosts:
- cert_expires: Aug 23 06:29:30 2026 GMT
  host: www.champ.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Champ Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Champ Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Champ Ai
provider_slug: champ-ai
slug: champ-ai-domain-security
source_filename: champ-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.champ.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:29:30 2026 GMT\n  hsts: false\ndomains:\n- domain: champ.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/champ-ai/refs/heads/main/security/champ-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Business Process Outsourcing
- Workflow Automation
- Document Intelligence
- Voice AI
- Healthcare
- Operations
---
