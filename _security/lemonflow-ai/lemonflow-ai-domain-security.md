---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lemonflow.ai
  spf: true
hosts:
- cert_expires: Oct  9 11:06:27 2026 GMT
  host: chat.lemonflow.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemonflow Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemonflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lemonflow
provider_slug: lemonflow-ai
slug: lemonflow-ai-domain-security
source_filename: lemonflow-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chat.lemonflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:06:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lemonflow.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonflow-ai/refs/heads/main/security/lemonflow-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Support
- Electric Vehicle Charging
- eMobility
- OCPP
- Chat Widget
- Voice
- Europe
---
