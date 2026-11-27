---
api_specs:
- filename: agentconnectors-dev-openapi.json
  format: json
  label: Agent Connectors API
  slug: agent-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentconnectors-dev/openapi/agentconnectors-dev-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentconnectors.dev
  spf: true
hosts:
- cert_expires: Jan 12 09:52:44 2027 GMT
  host: agentconnectors.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Connectors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Connectors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agent Connectors
provider_slug: agentconnectors-dev
slug: agentconnectors-dev-domain-security
source_filename: agentconnectors-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentconnectors.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 09:52:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentconnectors.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentconnectors-dev/security/agentconnectors-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Directory
- MCP
- Artificial Intelligence
- Open Data
- Public
---
