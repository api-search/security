---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: scalpstream.com
  spf: false
hosts:
- cert_expires: Oct 25 18:31:52 2026 GMT
  host: scalpstream.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 20:40:17 2026 GMT
  host: recallscout.scalpstream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 20:40:14 2026 GMT
  host: airscout.scalpstream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Scalpstream Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScalpStream, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: ScalpStream
provider_slug: scalpstream-com
slug: scalpstream-com-domain-security
source_filename: scalpstream-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scalpstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 18:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: recallscout.scalpstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 20:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: airscout.scalpstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 20:40:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scalpstream.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalpstream-com/refs/heads/main/security/scalpstream-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Agents
- A2A
- x402
- Micropayments
- MCP
- Open Data
- Product Recalls
- Air Quality
- Border Crossings
- Fuel Prices
- Market Research
- Public Safety
- Cryptocurrency
- USDC
- XRP Ledger
- llms-txt
- JSON Schema
---
