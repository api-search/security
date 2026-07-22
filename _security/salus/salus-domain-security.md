---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usesalus.ai
  spf: false
hosts:
- cert_expires: Aug 26 01:11:31 2026 GMT
  host: www.usesalus.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Salus
provider_slug: salus
slug: salus-domain-security
source_filename: salus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usesalus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:11:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usesalus.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salus/refs/heads/main/security/salus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Runtime Validation
- Agent Governance
- AI Safety
- Guardrails
- Developer Tools
- Infrastructure
---
