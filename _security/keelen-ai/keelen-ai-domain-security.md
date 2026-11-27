---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keelen.ai
  spf: true
hosts:
- cert_expires: Jan 18 11:35:20 2027 GMT
  host: keelen.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keelen AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keelen AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Keelen AI
provider_slug: keelen-ai
slug: keelen-ai-domain-security
source_filename: keelen-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keelen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 11:35:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keelen.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/keelen-ai/security/keelen-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Coding
- GitHub Integration
- Autonomous Agents
- Security isolation
- Internal Tools
---
