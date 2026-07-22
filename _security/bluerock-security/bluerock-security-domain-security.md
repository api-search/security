---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bluerock.io
  spf: true
hosts:
- cert_expires: Oct 15 21:07:40 2026 GMT
  host: www.bluerock.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluerock Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluerock Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bluerock Security
provider_slug: bluerock-security
slug: bluerock-security-domain-security
source_filename: bluerock-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluerock.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:07:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bluerock.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluerock-security/refs/heads/main/security/bluerock-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- AI Agents
- Agent Security
- MCP
- Model Context Protocol
- Observability
- Runtime Security
- AI Governance
- Guardrails
---
