---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epicgames.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: epicgames.dev
  spf: false
hosts:
- cert_expires: Aug 18 01:27:43 2026 GMT
  host: www.epicgames.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 01:58:57 2026 GMT
  host: dev.epicgames.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 17:29:26 2026 GMT
  host: api.epicgames.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epic Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epic Games, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Epic Games
provider_slug: epic-games
slug: epic-games-domain-security
source_filename: epic-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epicgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:27:43 2026 GMT\n  hsts: null\n- host: dev.epicgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:58:57 2026 GMT\n  hsts: false\n- host: api.epicgames.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:29:26 2026 GMT\n  hsts: null\ndomains:\n- domain: epicgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: epicgames.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-games/refs/heads/main/security/epic-games-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Achievements
- Anti-Cheat
- Cross-Platform
- EOS
- Epic Online Services
- Game Backend
- Game Development
- Games
- Identity
- Lobby
- Matchmaking
- Multiplayer
- Sessions
- Unreal Engine
- Voice
---
