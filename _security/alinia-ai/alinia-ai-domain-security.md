---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alinia.ai
  spf: true
hosts:
- cert_expires: Sep  6 14:33:14 2026 GMT
  host: alinia.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alinia Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alinia Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alinia Ai
provider_slug: alinia-ai
slug: alinia-ai-domain-security
source_filename: alinia-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alinia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:33:14 2026 GMT\n  hsts: false\ndomains:\n- domain: alinia.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alinia-ai/refs/heads/main/security/alinia-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Safety
- AI Compliance
- Guardrails
- LLM
- Governance
- Monitoring
- RegTech
---
