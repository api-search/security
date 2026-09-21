---
api_specs:
- filename: atomadic-tech-openapi.yml
  format: yaml
  label: AAAA Nexus API
  slug: aaaa-nexus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomadic-tech/refs/heads/main/openapi/atomadic-tech-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atomadic.tech
  spf: true
hosts:
- cert_expires: Oct 30 11:11:44 2026 GMT
  host: atomadic.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atomadic Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomadic Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atomadic Tech
provider_slug: atomadic-tech
slug: atomadic-tech-domain-security
source_filename: atomadic-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomadic.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 11:11:44 2026 GMT\n  hsts: false\ndomains:\n- domain: atomadic.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomadic-tech/refs/heads/main/security/atomadic-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Agents
- Agent Infrastructure
- MCP
- A2A
- x402
- Payments
- Compliance
- Security
- Trust
- Identity
- Escrow
- Inference
- Cryptography
---
