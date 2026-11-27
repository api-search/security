---
api_specs:
- filename: agent-preflight-com-api-openapi.json
  format: json
  label: Agent Preflight Api API
  slug: agent-preflight-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-preflight-com/openapi/_original/agent-preflight-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agent-preflight.com
  spf: false
hosts:
- cert_expires: Dec 16 23:05:33 2026 GMT
  host: agent-preflight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Preflight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Preflight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agent Preflight
provider_slug: agent-preflight-com
slug: agent-preflight-com-domain-security
source_filename: agent-preflight-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-preflight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:05:33 2026 GMT\n  hsts: false\ndomains:\n- domain: agent-preflight.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agent-preflight-com/security/agent-preflight-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Agents
- Preflight
- Tool
- Decisions
---
