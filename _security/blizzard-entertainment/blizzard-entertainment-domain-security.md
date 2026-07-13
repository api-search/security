---
api_specs:
- filename: blizzard-world-of-warcraft-openapi.yml
  format: yaml
  label: World of Warcraft Game Data API
  slug: world-of-warcraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-world-of-warcraft-openapi.yml
- filename: blizzard-diablo-iii-openapi.yml
  format: yaml
  label: Diablo III Community API
  slug: diablo-iii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-diablo-iii-openapi.yml
- filename: blizzard-starcraft-ii-openapi.yml
  format: yaml
  label: StarCraft II Community API
  slug: starcraft-ii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-starcraft-ii-openapi.yml
- filename: blizzard-hearthstone-openapi.yml
  format: yaml
  label: Hearthstone Game Data API
  slug: hearthstone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-hearthstone-openapi.yml
- filename: blizzard-oauth-openapi.yml
  format: yaml
  label: Battle.net OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/openapi/blizzard-oauth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blizzard.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: battle.net
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.blizzard.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: develop.battle.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: us.api.blizzard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blizzard Entertainment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blizzard Entertainment, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blizzard Entertainment
provider_slug: blizzard-entertainment
slug: blizzard-entertainment-domain-security
source_filename: blizzard-entertainment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blizzard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: develop.battle.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.api.blizzard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blizzard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: battle.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blizzard-entertainment/refs/heads/main/security/blizzard-entertainment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games
- Entertainment
- Video Games
- Game Data
- Battle.net
---
