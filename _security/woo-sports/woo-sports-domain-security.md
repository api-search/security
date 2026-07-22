---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: woosports.com
  spf: true
hosts:
- host: woosports.com
  https: false
kind: domain-security
layout: security
method: probed
name: Woo Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WOO Sports, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WOO Sports
provider_slug: woo-sports
slug: woo-sports-domain-security
source_filename: woo-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woosports.com\n  https: false\ndomains:\n- domain: woosports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woo-sports/refs/heads/main/security/woo-sports-domain-security.yml
summary_line: DMARC
tags:
- Company
- Sports
- Wearables
- IoT
- Sensors
- Kitesurfing
- Wingfoil
- GPS
- Fitness Tracking
- Community
- Leaderboards
---
