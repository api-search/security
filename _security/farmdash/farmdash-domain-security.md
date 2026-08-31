---
api_specs:
- filename: farmdash-account-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Account API
  slug: farmdash-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-account-api-openapi.yml
- filename: farmdash-autopilot-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Autopilot API
  slug: farmdash-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-autopilot-api-openapi.yml
- filename: farmdash-delegation-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Delegation API
  slug: farmdash-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-delegation-api-openapi.yml
- filename: farmdash-execution-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Execution API
  slug: farmdash-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-execution-api-openapi.yml
- filename: farmdash-history-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub History API
  slug: farmdash-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-history-api-openapi.yml
- filename: farmdash-intelligence-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Intelligence API
  slug: farmdash-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-intelligence-api-openapi.yml
- filename: farmdash-research-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Research API
  slug: farmdash-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-research-api-openapi.yml
- filename: farmdash-risk-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Risk API
  slug: farmdash-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-risk-api-openapi.yml
- filename: farmdash-session-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Session API
  slug: farmdash-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-session-api-openapi.yml
- filename: farmdash-strategy-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Strategy API
  slug: farmdash-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-strategy-api-openapi.yml
- filename: farmdash-swap-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Swap API
  slug: farmdash-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-swap-api-openapi.yml
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
