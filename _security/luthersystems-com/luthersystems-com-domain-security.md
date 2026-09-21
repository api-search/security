---
api_specs:
- filename: luthersystems-com-agentsearch-openapi.yml
  format: yaml
  label: AgentSearch HTTP API
  slug: agentsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luthersystems-com/refs/heads/main/openapi/luthersystems-com-agentsearch-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: luthersystems.com
  spf: true
hosts:
- cert_expires: Nov 21 19:31:17 2026 GMT
  host: luthersystems.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Luthersystems Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luther Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Luther Systems
provider_slug: luthersystems-com
slug: luthersystems-com-domain-security
source_filename: luthersystems-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luthersystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 19:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: luthersystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luthersystems-com/refs/heads/main/security/luthersystems-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agent Discovery
- MCP
- A2A
- agent-native
- Cloud Infrastructure
- Terraform
- Infrastructure as Code
- Process Automation
- Enterprise Automation
- Distributed Ledger
- Hyperledger Fabric
- Insurance
- Financial-Services
- Open-Source
---
