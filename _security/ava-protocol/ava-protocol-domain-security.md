---
api_specs:
- filename: ava-protocol-avs-openapi-original.yml
  format: yaml
  label: Ava Protocol AVS API
  slug: ava-protocol-avs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-avs-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avaprotocol.org
  spf: true
hosts:
- cert_expires: Oct  9 19:36:31 2026 GMT
  host: avaprotocol.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ava Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ava Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ava Protocol
provider_slug: ava-protocol
slug: ava-protocol-domain-security
source_filename: ava-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avaprotocol.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avaprotocol.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/security/ava-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Blockchain
- DeFi
- Automation
- Web3
- Ethereum
- Smart Wallets
- Workflows
- AI Agents
---
