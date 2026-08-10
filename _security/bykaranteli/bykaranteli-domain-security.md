---
api_specs:
- filename: bykaranteli-x402-api-openapi.yml
  format: yaml
  label: ByKaranteli X402 API
  slug: bykaranteli-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/openapi/bykaranteli-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bykaranteli.com
  spf: true
hosts:
- cert_expires: Sep 20 18:28:00 2026 GMT
  host: bykaranteli.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bykaranteli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByKaranteli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ByKaranteli
provider_slug: bykaranteli
slug: bykaranteli-domain-security
source_filename: bykaranteli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bykaranteli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bykaranteli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/security/bykaranteli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Crypto Derivatives
- Market Data
- Funding Rates
- Open Interest
- Liquidations
- Options
- ETF Flows
- Financial Data
- MCP
- x402
- Agents
---
