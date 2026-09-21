---
api_specs:
- filename: open-poker-openapi.json
  format: json
  label: Open Poker REST API
  slug: open-poker-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-poker/refs/heads/main/openapi/open-poker-openapi.json
- filename: open-poker-websocket-asyncapi.yml
  format: yaml
  label: Open Poker WebSocket Game API
  slug: open-poker-websocket-game-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-poker/refs/heads/main/asyncapi/open-poker-websocket-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openpoker.ai
  spf: true
hosts:
- cert_expires: Nov 25 12:20:18 2026 GMT
  host: docs.openpoker.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 12:20:18 2026 GMT
  host: api.openpoker.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 12:20:18 2026 GMT
  host: openpoker.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Open Poker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Poker, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Poker
provider_slug: open-poker
slug: open-poker-domain-security
source_filename: open-poker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.openpoker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 12:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openpoker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 12:20:18 2026 GMT\n  hsts: null\n- host: openpoker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 12:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openpoker.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-poker/refs/heads/main/security/open-poker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Poker
- Artificial Intelligence
- Autonomous Agents
- Developer Tools
- WebSocket
- Real-Time
- Leaderboards
- Competitions
- bot-infrastructure
---
