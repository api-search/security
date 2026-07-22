---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: artian.ai
  spf: true
hosts:
- cert_expires: Aug 23 16:17:53 2026 GMT
  host: artian.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Artian
provider_slug: artian
slug: artian-domain-security
source_filename: artian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artian.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 16:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: artian.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artian/refs/heads/main/security/artian-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic AI
- Financial Services
- Enterprise Software
- Workflow Automation
- AI Governance
- Model Risk Management
- Insurance
---
