---
api_specs:
- filename: loot-rush-games-partner-openapi.json
  format: json
  label: LootRush Partner API
  slug: lootrush-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loot-rush-games/refs/heads/main/openapi/loot-rush-games-partner-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lootrush.com
  spf: false
hosts:
- cert_expires: Aug 31 15:09:44 2026 GMT
  host: www.lootrush.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 15:09:44 2026 GMT
  host: docs.lootrush.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 15:09:44 2026 GMT
  host: third-party.lootrush.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loot Rush Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loot Rush Games, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Loot Rush Games
provider_slug: loot-rush-games
slug: loot-rush-games-domain-security
source_filename: loot-rush-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lootrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:09:44 2026 GMT\n  hsts: null\n- host: docs.lootrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:09:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: third-party.lootrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:09:44 2026 GMT\n  hsts: null\ndomains:\n- domain: lootrush.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loot-rush-games/refs/heads/main/security/loot-rush-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Blockchain
- Gaming
- Fintech
- Wallets
- Cards
- Payments
- Withdrawals
- MCP
- Agent-Ready
---
