---
api_specs:
- filename: scott-ai-openapi-original.json
  format: json
  label: Scott One-Shot API
  slug: scott-one-shot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scott-ai/refs/heads/main/openapi/scott-ai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryscott.ai
  spf: true
hosts:
- cert_expires: Sep 24 07:30:13 2026 GMT
  host: tryscott.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:30:12 2026 GMT
  host: docs.tryscott.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.tryscott.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Scott Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scott Ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scott Ai
provider_slug: scott-ai
slug: scott-ai-domain-security
source_filename: scott-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryscott.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 07:30:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tryscott.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:30:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tryscott.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tryscott.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scott-ai/refs/heads/main/security/scott-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coding Agents
- AI
- Developer Tools
- Collaboration
- Agentic Workflow
- Model Context Protocol
- Software Design
---
