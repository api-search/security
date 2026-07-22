---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 7ai.com
  spf: true
hosts:
- cert_expires: Oct  5 06:08:25 2026 GMT
  host: 7ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 7Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 7AI
provider_slug: 7ai
slug: 7ai-domain-security
source_filename: 7ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 7ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 06:08:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 7ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7ai/refs/heads/main/security/7ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Security
- Artificial Intelligence
- AI Agents
- Agentic Security
- Security Operations
- SOC
- Threat Detection
- Incident Response
---
