---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: board.fun
  spf: true
hosts:
- cert_expires: Sep  2 19:08:31 2026 GMT
  host: board.fun
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Board
provider_slug: board
slug: board-domain-security
source_filename: board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: board.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 19:08:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: board.fun\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/board/refs/heads/main/security/board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Board Games
- Agent Commerce
- Universal Commerce Protocol
- Shopify
- MCP
---
