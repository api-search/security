---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: playhouse.so
  spf: true
hosts:
- host: playhouse.so
  https: false
kind: domain-security
layout: security
method: probed
name: Playhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for playhouse, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: playhouse
provider_slug: playhouse
slug: playhouse-domain-security
source_filename: playhouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playhouse.so\n  https: false\ndomains:\n- domain: playhouse.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playhouse/refs/heads/main/security/playhouse-domain-security.yml
summary_line: DMARC
tags:
- Company
- Real Estate
- PropTech
- Mobile App
- Consumer
- Listings
- Polls
---
