---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: igent.ai
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: igent.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 22:20:02 2026 GMT
  host: docs.igent.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Igent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iGent, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iGent
provider_slug: igent
slug: igent-domain-security
source_filename: igent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: igent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: docs.igent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: igent.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igent/refs/heads/main/security/igent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Artificial Intelligence
- Software Development
- Coding Agent
- Developer Tools
- AI Agents
- Automation
- LLM
- Cloud Sandbox
---
