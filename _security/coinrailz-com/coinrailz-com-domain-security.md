---
api_specs:
- filename: coinrailz-com-agent-payment-api-openapi.yml
  format: yaml
  label: Coin Railz Agent Payment API
  slug: agent-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinrailz-com/refs/heads/main/openapi/coinrailz-com-agent-payment-api-openapi.yml
- filename: coinrailz-com-x402-services-openapi.yml
  format: yaml
  label: Coin Railz x402 Micropayment Services
  slug: x402-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinrailz-com/refs/heads/main/openapi/coinrailz-com-x402-services-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coinrailz.com
  spf: true
hosts:
- cert_expires: Oct 18 22:09:53 2026 GMT
  host: coinrailz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinrailz Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coin Railz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coin Railz
provider_slug: coinrailz-com
slug: coinrailz-com-domain-security
source_filename: coinrailz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinrailz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:09:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coinrailz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinrailz-com/refs/heads/main/security/coinrailz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Agents
- x402
- Micropayments
- Cryptocurrency
- DeFi
- Blockchain
- Stablecoins
- USDC
- Prediction Markets
- Satellite Data
- IoT
- Trading
- Compliance
- MCP
- A2A
---
