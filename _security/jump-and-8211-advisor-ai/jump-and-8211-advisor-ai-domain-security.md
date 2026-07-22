---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jump.ai
  spf: false
hosts:
- cert_expires: Sep 28 23:30:31 2026 GMT
  host: jump.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jump And 8211 Advisor Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jump &#8211; Advisor AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Jump &#8211; Advisor AI
provider_slug: jump-and-8211-advisor-ai
slug: jump-and-8211-advisor-ai-domain-security
source_filename: jump-and-8211-advisor-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jump.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:30:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jump.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jump-and-8211-advisor-ai/refs/heads/main/security/jump-and-8211-advisor-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Financial Advisors
- Wealth Management
- Fintech
- AI Assistant
- Meeting Notes
- Integrations
---
