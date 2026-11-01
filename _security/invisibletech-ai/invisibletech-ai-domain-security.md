---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: invisibletech.ai
  spf: true
hosts:
- cert_expires: Jan 19 23:15:01 2027 GMT
  host: invisibletech.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Invisibletech Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invisible Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Invisible Technologies
provider_slug: invisibletech-ai
slug: invisibletech-ai-domain-security
source_filename: invisibletech-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invisibletech.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:15:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: invisibletech.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/invisibletech-ai/security/invisibletech-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Training Data
- Reinforcement Learning
- Enterprise AI
- Automation
- AI Agents
---
