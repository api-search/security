---
description: ''
domains:
- caa:
  - hk836.pc51.com.
  dmarc: false
  dnssec: true
  domain: forgame.com
  spf: true
hosts:
- host: forgame.com
  https: false
kind: domain-security
layout: security
method: probed
name: Forgame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for forgame, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: forgame
provider_slug: forgame
slug: forgame-domain-security
source_filename: forgame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgame.com\n  https: false\ndomains:\n- domain: forgame.com\n  dnssec: true\n  caa:\n  - hk836.pc51.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forgame/refs/heads/main/security/forgame-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Gaming
- Cloud Gaming
- Web Games
- Mobile Games
- Fintech
- E-Sports
- China
---
