---
api_specs:
- filename: activision-blizzard-account-api-openapi.yml
  format: yaml
  label: activision-blizzard Account API
  slug: activision-blizzard-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/openapi/activision-blizzard-account-api-openapi.yml
- filename: activision-blizzard-diablo-iii-api-openapi.yml
  format: yaml
  label: activision-blizzard Diablo III API
  slug: activision-blizzard-diablo-iii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/openapi/activision-blizzard-diablo-iii-api-openapi.yml
- filename: activision-blizzard-hearthstone-api-openapi.yml
  format: yaml
  label: activision-blizzard Hearthstone API
  slug: activision-blizzard-hearthstone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/openapi/activision-blizzard-hearthstone-api-openapi.yml
- filename: activision-blizzard-starcraft-ii-api-openapi.yml
  format: yaml
  label: activision-blizzard StarCraft II API
  slug: activision-blizzard-starcraft-ii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/openapi/activision-blizzard-starcraft-ii-api-openapi.yml
- filename: activision-blizzard-world-of-warcraft-api-openapi.yml
  format: yaml
  label: activision-blizzard World of Warcraft API
  slug: activision-blizzard-world-of-warcraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/openapi/activision-blizzard-world-of-warcraft-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: activision-blizzard.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: battle.net
  spf: true
hosts:
- host: www.activision-blizzard.com
  https: false
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: develop.battle.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: gateway.battlenet.com.cn
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Activision Blizzard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for activision-blizzard, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: activision-blizzard
provider_slug: activision-blizzard
slug: activision-blizzard-domain-security
source_filename: activision-blizzard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activision-blizzard.com\n  https: false\n- host: develop.battle.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.battlenet.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: activision-blizzard.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: battle.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/security/activision-blizzard-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fortune 1000
---
