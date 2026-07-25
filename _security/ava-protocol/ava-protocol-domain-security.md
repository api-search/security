---
api_specs:
- filename: ava-protocol-auth-api-openapi.yml
  format: yaml
  label: Ava Protocol Auth API
  slug: ava-protocol-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-auth-api-openapi.yml
- filename: ava-protocol-executions-api-openapi.yml
  format: yaml
  label: Ava Protocol Executions API
  slug: ava-protocol-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-executions-api-openapi.yml
- filename: ava-protocol-health-api-openapi.yml
  format: yaml
  label: Ava Protocol Health API
  slug: ava-protocol-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-health-api-openapi.yml
- filename: ava-protocol-nodes-api-openapi.yml
  format: yaml
  label: Ava Protocol Nodes API
  slug: ava-protocol-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-nodes-api-openapi.yml
- filename: ava-protocol-operators-api-openapi.yml
  format: yaml
  label: Ava Protocol Operators API
  slug: ava-protocol-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-operators-api-openapi.yml
- filename: ava-protocol-secrets-api-openapi.yml
  format: yaml
  label: Ava Protocol Secrets API
  slug: ava-protocol-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-secrets-api-openapi.yml
- filename: ava-protocol-tokens-api-openapi.yml
  format: yaml
  label: Ava Protocol Tokens API
  slug: ava-protocol-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-tokens-api-openapi.yml
- filename: ava-protocol-triggers-api-openapi.yml
  format: yaml
  label: Ava Protocol Triggers API
  slug: ava-protocol-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-triggers-api-openapi.yml
- filename: ava-protocol-wallets-api-openapi.yml
  format: yaml
  label: Ava Protocol Wallets API
  slug: ava-protocol-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-wallets-api-openapi.yml
- filename: ava-protocol-workflows-api-openapi.yml
  format: yaml
  label: Ava Protocol Workflows API
  slug: ava-protocol-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-protocol/refs/heads/main/openapi/ava-protocol-workflows-api-openapi.yml
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
