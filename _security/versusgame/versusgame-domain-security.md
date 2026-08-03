---
api_specs:
- filename: versusgame-openapi-original.json
  format: json
  label: Versusgame API
  slug: versusgame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/versusgame/refs/heads/main/openapi/versusgame-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: versusgame.com
  spf: true
hosts:
- cert_expires: Oct  1 12:39:45 2026 GMT
  host: www.versusgame.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.versusgame.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Versusgame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VersusGame, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VersusGame
provider_slug: versusgame
slug: versusgame-domain-security
source_filename: versusgame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.versusgame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:39:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.versusgame.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: versusgame.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versusgame/refs/heads/main/security/versusgame-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- gaming
- prediction-games
- audience-engagement
- gamification
- media-and-entertainment
- publishing
- widgets
- leaderboards
- creator-economy
- ai-content-generation
- payments
---
