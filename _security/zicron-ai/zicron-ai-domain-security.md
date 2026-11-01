---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zicron.ai
  spf: true
hosts:
- host: zicron.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zicron Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zicron-ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: zicron-ai
provider_slug: zicron-ai
slug: zicron-ai-domain-security
source_filename: zicron-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zicron.ai\n  https: false\ndomains:\n- domain: zicron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zicron-ai/security/zicron-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
- AI
- Productivity
- Knowledge-Management
- SaaS
- Startup
---
