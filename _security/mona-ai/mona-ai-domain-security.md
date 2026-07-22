---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mona-ai.de
  spf: true
hosts:
- cert_expires: Oct 14 17:03:13 2026 GMT
  host: www.mona-ai.de
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mona Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mona Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mona Ai
provider_slug: mona-ai
slug: mona-ai-domain-security
source_filename: mona-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mona-ai.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:03:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: mona-ai.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mona-ai/refs/heads/main/security/mona-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Human Resources
- HR Tech
- AI Agents
- Automation
- Germany
- MCP
---
