---
api_specs:
- filename: coval-agents-openapi.yml
  format: yaml
  label: Coval API
  slug: coval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval/refs/heads/main/openapi/coval-agents-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coval.dev
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.coval.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coval, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coval
provider_slug: coval
slug: coval-domain-security
source_filename: coval-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.coval.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coval.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coval/refs/heads/main/security/coval-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- AI Agents
- Voice AI
- Testing
- Evaluation
- Simulation
- Observability
- Conversational AI
- LLM
- Quality Assurance
---
