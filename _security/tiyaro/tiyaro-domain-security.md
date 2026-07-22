---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tiyaro.ai
  spf: true
hosts:
- cert_expires: Sep 25 15:42:43 2026 GMT
  host: www.tiyaro.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiyaro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiyaro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tiyaro
provider_slug: tiyaro
slug: tiyaro-domain-security
source_filename: tiyaro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiyaro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:42:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: tiyaro.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiyaro/refs/heads/main/security/tiyaro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic AI
- Customer Support
- IT Service Management
- Business Process Automation
- Enterprise Software
- LLM
- Revenue Operations
---
