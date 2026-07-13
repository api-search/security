---
api_specs:
- filename: stackmint-openapi.yml
  format: yaml
  label: Stackmint Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackmint/refs/heads/main/openapi/stackmint-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stackmint.ai
  spf: true
hosts:
- cert_expires: Oct  4 12:12:23 2026 GMT
  host: stackmint.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.stackmint.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Stackmint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stackmint, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stackmint
provider_slug: stackmint
slug: stackmint-domain-security
source_filename: stackmint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackmint.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:12:23 2026 GMT\n  hsts: false\n- host: api.stackmint.ai\n  https: false\ndomains:\n- domain: stackmint.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackmint/refs/heads/main/security/stackmint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Governance
- AI Agents
- Workflow Automation
- Enterprise AI
- MCP
- Semantic Layer
- Audit
- Compliance
---
