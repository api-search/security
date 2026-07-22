---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: taito.ai
  spf: true
hosts:
- cert_expires: Sep  6 10:01:19 2026 GMT
  host: taito.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taitoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taito.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Taito.ai
provider_slug: taitoai
slug: taitoai-domain-security
source_filename: taitoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taito.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 10:01:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: taito.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taitoai/refs/heads/main/security/taitoai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- HR
- People Operations
- HRIS
- Performance Management
- Employee Experience
- AI Agents
- MCP
- SaaS
- GDPR
- ISO 27001
---
