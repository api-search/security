---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diezx.ai
  spf: true
hosts:
- host: diezx.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diezx Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for diezX, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: diezX
provider_slug: diezx-ai
slug: diezx-ai-domain-security
source_filename: diezx-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diezx.ai\n  https: false\ndomains:\n- domain: diezx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/diezx-ai/security/diezx-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Business Observability
- AI Agents
- MCP
- Process Automation
- Accounts Payable
- Sales Analytics
- Small Business
---
