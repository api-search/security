---
api_specs:
- filename: farmdash-agent-api-openapi.yaml
  format: yaml
  label: FarmDash Agent Hub API
  slug: farmdash-agent-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-agent-api-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: farmdash.one
  spf: true
hosts:
- cert_expires: Nov 18 23:35:01 2026 GMT
  host: www.farmdash.one
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Farmdash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FarmDash Agent Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FarmDash Agent Hub
provider_slug: farmdash
slug: farmdash-domain-security
source_filename: farmdash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.farmdash.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:35:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: farmdash.one\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/security/farmdash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- DeFAI
- AI agents
- MCP
- OpenAPI
- x402
- blockchain
- crypto
- airdrop tracking
- developer tools
- agent readiness
- machine payments
- Hyperliquid
- wallet intelligence
- zero custody
---
