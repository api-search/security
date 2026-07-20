---
api_specs:
- filename: end-game-openapi.json
  format: json
  label: Endgame Public API
  slug: endgame-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: endgame.io
  spf: true
hosts:
- cert_expires: Oct 15 14:26:38 2026 GMT
  host: www.endgame.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 03:46:45 2026 GMT
  host: docs.endgame.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 13:35:12 2026 GMT
  host: app.endgame.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: End Game Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endgame, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Endgame
provider_slug: end-game
slug: end-game-domain-security
source_filename: end-game-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endgame.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:26:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.endgame.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 03:46:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.endgame.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:35:12 2026 GMT\n  hsts: false\ndomains:\n- domain: endgame.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/security/end-game-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- Revenue Intelligence
- Go-To-Market
- Artificial Intelligence
- Agents
- MCP
- Knowledge Graph
- CRM
- Conversation Intelligence
---
