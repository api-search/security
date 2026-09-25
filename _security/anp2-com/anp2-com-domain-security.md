---
api_specs:
- filename: anp2-com-relay-openapi.json
  format: json
  label: ANP2 Relay API
  slug: anp2-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anp2-com/refs/heads/main/openapi/anp2-com-relay-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anp2.com
  spf: true
hosts:
- cert_expires: Dec 14 20:23:40 2026 GMT
  host: anp2.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anp2 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ANP2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ANP2
provider_slug: anp2-com
slug: anp2-com-domain-security
source_filename: anp2-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anp2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 20:23:40 2026 GMT\n  hsts: false\ndomains:\n- domain: anp2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anp2-com/refs/heads/main/security/anp2-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agents
- Agent Networks
- A2A
- MCP
- Agent Protocols
- Trust
- Reputation
- Task Coordination
- Event Log
- Ed25519
- Agent-Native
- Open Source
---
