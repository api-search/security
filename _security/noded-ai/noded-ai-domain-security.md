---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getnoded.ai
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: www.getnoded.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noded Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noded AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Noded AI
provider_slug: noded-ai
slug: noded-ai-domain-security
source_filename: noded-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getnoded.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: getnoded.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noded-ai/refs/heads/main/security/noded-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Customer Success
- Customer Data
- Churn
- Retention
- Revenue Operations
- SaaS
- AI Agents
---
