---
api_specs:
- filename: riot-games-league-of-legends-openapi.yml
  format: yaml
  label: League of Legends API
  slug: league-of-legends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/openapi/riot-games-league-of-legends-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: riotgames.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.riotgames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 05:49:40 2026 GMT
  host: developer.riotgames.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 05:54:17 2026 GMT
  host: na1.api.riotgames.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riot Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riot Games, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Riot Games
provider_slug: riot-games
slug: riot-games-domain-security
source_filename: riot-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riotgames.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.riotgames.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 05:49:40 2026 GMT\n  hsts: false\n- host: na1.api.riotgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 05:54:17 2026 GMT\n  hsts: null\ndomains:\n- domain: riotgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/security/riot-games-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Esports
- Gaming
- League of Legends
- Legends of Runeterra
- Teamfight Tactics
- VALORANT
---
