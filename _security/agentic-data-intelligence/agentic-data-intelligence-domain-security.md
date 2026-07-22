---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentic-data.com
  spf: true
hosts:
- cert_expires: Oct  5 16:18:29 2026 GMT
  host: agentic-data.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentic Data Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentic Data Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agentic Data Intelligence
provider_slug: agentic-data-intelligence
slug: agentic-data-intelligence-domain-security
source_filename: agentic-data-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentic-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:18:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentic-data.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentic-data-intelligence/refs/heads/main/security/agentic-data-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Data Analytics
- Agents
- MCP
- Agent Skills
- Semantics
- Data Governance
- Semantic Layer
- Data Intelligence
---
