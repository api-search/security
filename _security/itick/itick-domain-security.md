---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: itick.org
  spf: true
hosts:
- cert_expires: Nov 24 15:25:14 2026 GMT
  host: docs.itick.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 15:25:14 2026 GMT
  host: api.itick.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Itick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iTick, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: iTick
provider_slug: itick
slug: itick-domain-security
source_filename: itick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.itick.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 15:25:14 2026 GMT\n  hsts: false\n- host: api.itick.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 15:25:14 2026 GMT\n  hsts: null\ndomains:\n- domain: itick.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itick/refs/heads/main/security/itick-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial Data
- Market Data
- Stocks
- Forex
- Crypto
- Indices
- Futures
- Fund
- Real-Time Data
- WebSocket
- FIX Protocol
- Fintech
- Quantitative Trading
- MCP Server
---
