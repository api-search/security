---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: botco.ai
  spf: true
hosts:
- cert_expires: Dec  7 06:04:44 2026 GMT
  host: botco.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botco Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botco.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Botco.ai
provider_slug: botco-ai
slug: botco-ai-domain-security
source_filename: botco-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botco.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 06:04:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: botco.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botco-ai/refs/heads/main/security/botco-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Chatbots
- Healthcare
- Pharmaceuticals
- Government
- Compliance
- Software-as-a-Service
---
