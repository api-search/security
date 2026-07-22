---
api_specs:
- filename: ressl-ai-platform-openapi.yml
  format: yaml
  label: Ressl Platform API
  slug: ressl-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ressl-ai/refs/heads/main/openapi/ressl-ai-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ressl.ai
  spf: true
hosts:
- cert_expires: Sep 20 10:30:19 2026 GMT
  host: simulation.ressl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ressl Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ressl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ressl
provider_slug: ressl-ai
slug: ressl-ai-domain-security
source_filename: ressl-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simulation.ressl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 10:30:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ressl.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ressl-ai/refs/heads/main/security/ressl-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mock APIs
- API Testing
- AI Agents
- Agent Evaluation
- Sandbox
- Developer Tools
- Synthetic Data
- SaaS
---
