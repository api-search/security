---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: betgenius.com
  spf: true
hosts:
- host: www.betgenius.com
  https: false
kind: domain-security
layout: security
method: probed
name: Betgenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetGenius, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BetGenius
provider_slug: betgenius
slug: betgenius-domain-security
source_filename: betgenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betgenius.com\n  https: false\ndomains:\n- domain: betgenius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/security/betgenius-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Sportsbook
- Sports Betting
- Sports Data
- Odds Feeds
- Trading Services
- Risk Management
- Live Streaming
- In-Play Betting
- BetBuilder
- Player Engagement
- Marketing Technology
- Gambling
---
