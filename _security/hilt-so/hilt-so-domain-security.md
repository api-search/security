---
api_specs:
- filename: hilt-so-openapi.yml
  format: yaml
  label: Hilt API (Pay API + Workspace)
  slug: hilt-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/openapi/hilt-so-openapi.yml
- filename: hilt-so-transaction-evidence-openapi.yml
  format: yaml
  label: Hilt Solana Transaction Evidence API
  slug: transaction-evidence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/openapi/hilt-so-transaction-evidence-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hilt.so
  spf: false
hosts:
- cert_expires: Nov 21 18:35:49 2026 GMT
  host: hilt.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hilt So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hilt
provider_slug: hilt-so
slug: hilt-so-domain-security
source_filename: hilt-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hilt.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:35:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hilt.so\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilt-so/refs/heads/main/security/hilt-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Solana
- Stablecoins
- USDC
- Crypto Payments
- Agentic Payments
- x402
- Checkout
- Subscription
- Webhook
- MCP
- Entitlements
- Micropayments
- Developer Tools
- Fintech
- A2A
---
