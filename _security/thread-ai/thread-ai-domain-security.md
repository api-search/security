---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: threadai.com
  spf: true
hosts:
- cert_expires: Oct  3 13:46:31 2026 GMT
  host: www.threadai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thread Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thread AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thread AI
provider_slug: thread-ai
slug: thread-ai-domain-security
source_filename: thread-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.threadai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: threadai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thread-ai/refs/heads/main/security/thread-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- AI Orchestration
- Workflow Automation
- Agents
- Enterprise
- Governance
- MLOps
---
