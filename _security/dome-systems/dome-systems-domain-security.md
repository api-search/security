---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: domesystems.ai
  spf: true
hosts:
- cert_expires: Sep  4 10:46:59 2026 GMT
  host: www.domesystems.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dome Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dome Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dome Systems
provider_slug: dome-systems
slug: dome-systems-domain-security
source_filename: dome-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domesystems.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:46:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: domesystems.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dome-systems/refs/heads/main/security/dome-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agent Governance
- AI Operations
- Authorization
- Audit
- MCP
- Enterprise
- Cedar Policy
- LLM
---
