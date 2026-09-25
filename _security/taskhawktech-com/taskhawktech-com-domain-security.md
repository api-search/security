---
api_specs:
- filename: taskhawktech-com-openapi.yml
  format: yaml
  label: Kevros Governance API
  slug: kevros-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskhawktech-com/refs/heads/main/openapi/taskhawktech-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: taskhawktech.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: taskhawktech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: governance.taskhawktech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Taskhawktech Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaskHawk Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TaskHawk Systems
provider_slug: taskhawktech-com
slug: taskhawktech-com-domain-security
source_filename: taskhawktech-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taskhawktech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: governance.taskhawktech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: taskhawktech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskhawktech-com/refs/heads/main/security/taskhawktech-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Governance
- Agent Security
- Runtime Enforcement
- Policy Enforcement
- Provenance
- Compliance
- Prompt Injection Detection
- Media Attestation
- Post-Quantum Cryptography
- Formal Verification
- x402
- L402
- Machine Payments
- MCP
- A2A
- Agent-Native
- Government
- Defense
---
