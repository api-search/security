---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jeeva.ai
  spf: true
hosts:
- cert_expires: Oct  7 04:12:21 2026 GMT
  host: www.jeeva.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jeeva Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jeeva AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jeeva AI
provider_slug: jeeva-ai
slug: jeeva-ai-domain-security
source_filename: jeeva-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jeeva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:12:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jeeva.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeeva-ai/refs/heads/main/security/jeeva-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- AI Agents
- Digital Workers
- Sales Automation
- Revenue Operations
- No-Code
- Automation
---
