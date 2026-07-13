---
api_specs:
- filename: battle-net-hearthstone-game-data.yaml
  format: yaml
  label: Hearthstone Game Data API
  slug: hearthstone-game-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/openapi/battle-net-hearthstone-game-data.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: battle.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blizzard.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: community.developer.battle.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: us.api.blizzard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: eu.api.blizzard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Battle Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Battle.net, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Battle.net
provider_slug: battle-net
slug: battle-net-domain-security
source_filename: battle-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.developer.battle.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.api.blizzard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\n- host: eu.api.blizzard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: battle.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: blizzard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/security/battle-net-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
---
