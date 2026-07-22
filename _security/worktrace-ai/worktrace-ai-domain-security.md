---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: worktrace.ai
  spf: true
hosts:
- cert_expires: Aug 31 15:37:11 2026 GMT
  host: worktrace.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worktrace Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worktrace AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Worktrace AI
provider_slug: worktrace-ai
slug: worktrace-ai-domain-security
source_filename: worktrace-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worktrace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:37:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: worktrace.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worktrace-ai/refs/heads/main/security/worktrace-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Workflow Automation
- Artificial Intelligence
- Process Intelligence
- Enterprise
- Agents
---
