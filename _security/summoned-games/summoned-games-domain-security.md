---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: summoned.games
  spf: true
hosts:
- cert_expires: Dec 30 05:01:04 2026 GMT
  host: summoned.games
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Summoned Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Summoned Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Summoned Games
provider_slug: summoned-games
slug: summoned-games-domain-security
source_filename: summoned-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: summoned.games\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 05:01:04 2026 GMT\n  hsts: false\ndomains:\n- domain: summoned.games\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/summoned-games/security/summoned-games-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Browser
- AI
- Free
- Multiplayer
---
