---
api_specs:
- filename: cognition-openapi.yml
  format: yaml
  label: Devin API
  slug: devin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/openapi/cognition-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognition.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: devin.ai
  spf: true
hosts:
- cert_expires: Sep 15 04:25:43 2026 GMT
  host: cognition.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 22:34:00 2026 GMT
  host: docs.devin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api.devin.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognition AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cognition AI
provider_slug: cognition
slug: cognition-domain-security
source_filename: cognition-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognition.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:25:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.devin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 22:34:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.devin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cognition.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: devin.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognition/refs/heads/main/security/cognition-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Agents
- AI Software Engineer
- Coding Agents
- Developer Productivity
- DevOps
- Code Migration
- Code Review
- GitHub Integration
- Enterprise AI
- Agentic Workflows
- IDE
- LLM Applications
---
