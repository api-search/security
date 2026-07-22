---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigsur.ai
  spf: true
hosts:
- host: bigsur.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Big Sur Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Sur Ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Big Sur Ai
provider_slug: big-sur-ai
slug: big-sur-ai-domain-security
source_filename: big-sur-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigsur.ai\n  https: false\ndomains:\n- domain: bigsur.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-sur-ai/refs/heads/main/security/big-sur-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Conversational AI
- Shopping Assistant
- Retail Technology
- SaaS
- Sales Agent
---
