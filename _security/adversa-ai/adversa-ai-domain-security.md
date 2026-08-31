---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adversa.ai
  spf: true
hosts:
- cert_expires: Oct 13 11:45:12 2026 GMT
  host: adversa.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adversa Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adversa AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adversa AI
provider_slug: adversa-ai
slug: adversa-ai-domain-security
source_filename: adversa-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adversa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:45:12 2026 GMT\n  hsts: false\ndomains:\n- domain: adversa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adversa-ai/refs/heads/main/security/adversa-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Security
- AI Red Teaming
- LLM Security
- Agentic AI
- Adversarial Machine Learning
- AI Governance
- Cybersecurity
---
