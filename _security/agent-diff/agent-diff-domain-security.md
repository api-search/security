---
api_specs:
- filename: agent-diff-sandbox-openapi.yml
  format: yaml
  label: Agent Diff Sandbox API
  slug: agent-diff-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/openapi/agent-diff-sandbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentdiff.dev
  spf: false
hosts:
- cert_expires: Sep  6 17:42:52 2026 GMT
  host: www.agentdiff.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 15:08:42 2026 GMT
  host: api.agentdiff.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agent Diff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Diff, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Agent Diff
provider_slug: agent-diff
slug: agent-diff-domain-security
source_filename: agent-diff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentdiff.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:42:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.agentdiff.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:08:42 2026 GMT\n  hsts: null\ndomains:\n- domain: agentdiff.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/security/agent-diff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
---
