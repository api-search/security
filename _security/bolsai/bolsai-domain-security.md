---
api_specs:
- filename: openapi.json
  format: json
  label: Bolsai Financial Data API
  slug: bolsai-financial-data-api
  spec_type: OpenAPI
  url: https://usebolsai.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usebolsai.com
  spf: true
hosts:
- cert_expires: Oct 18 15:25:29 2026 GMT
  host: usebolsai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 15:25:29 2026 GMT
  host: api.usebolsai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bolsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolsai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bolsai
provider_slug: bolsai
slug: bolsai-domain-security
source_filename: bolsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usebolsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:25:29 2026 GMT\n  hsts: false\n- host: api.usebolsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:25:29 2026 GMT\n  hsts: false\ndomains:\n- domain: usebolsai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/security/bolsai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Financial Data
- Market Data
- Stocks/equities
- Real Estate Funds
- Dividends
- Fundamentals
- Macroeconomic Data
- Brazil
- Developer Tools
- MCP
- AI Agents
---
