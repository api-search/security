---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thedroneracingleague.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: dmarc-reports@drl.io
  dnssec: false
  domain: drl.io
  spf: true
hosts:
- host: thedroneracingleague.com
  https: false
  note: TLS handshake rejected by the origin (tlsv1 alert internal error); no certificate presented on 2026-08-04
- host: www.drl.io
  https: false
  note: CNAME to proxy-ssl.webflow.com; TLS handshake failure on client hello, no certificate presented on 2026-08-04
- host: drl.io
  https: false
  note: TLS handshake rejected by the origin; HTTP 301 to https:// which then fails
- host: metaverse.drl.io
  https: true
  note: Cloudflare Pages SPA ("DRL Interactive Marathon"); returns 200 text/html for every path probed, including /openapi.json - catch-all, not an API
- host: api.nft.drl.io
  http_status: 503
  https: true
  note: Google-hosted; 503 on every path probed - decommissioned NFT platform API host
kind: domain-security
layout: security
method: probed
name: Drone Racing League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drone Racing League, probed live across 5 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Drone Racing League
provider_slug: drone-racing-league
slug: drone-racing-league-domain-security
source_filename: drone-racing-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thedroneracingleague.com\n  https: false\n  note: TLS handshake rejected by the origin (tlsv1 alert internal error); no certificate\n    presented on 2026-08-04\n- host: www.drl.io\n  https: false\n  note: CNAME to proxy-ssl.webflow.com; TLS handshake failure on client hello, no certificate\n    presented on 2026-08-04\n- host: drl.io\n  https: false\n  note: TLS handshake rejected by the origin; HTTP 301 to https:// which then fails\n- host: metaverse.drl.io\n  https: true\n  note: Cloudflare Pages SPA (\"DRL Interactive Marathon\"); returns 200 text/html for every\n    path probed, including /openapi.json - catch-all, not an API\n- host: api.nft.drl.io\n  https: true\n  http_status: 503\n  note: Google-hosted; 503 on every path probed - decommissioned NFT platform API host\ndomains:\n- domain: thedroneracingleague.com\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: none\n- domain: drl.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: dmarc-reports@drl.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drone-racing-league/refs/heads/main/security/drone-racing-league-domain-security.yml
summary_line: DMARC
tags:
- Company
- Sports
- Esports
- Drones
- Racing
- Media
- Entertainment
- Broadcasting
- Gaming
- Simulation
---
