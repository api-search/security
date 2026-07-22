---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: topxgun.com
  spf: true
hosts:
- host: www.topxgun.com
  https: false
kind: domain-security
layout: security
method: probed
name: Topxgun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TopXGun, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TopXGun
provider_slug: topxgun
slug: topxgun-domain-security
source_filename: topxgun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.topxgun.com\n  https: false\ndomains:\n- domain: topxgun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topxgun/refs/heads/main/security/topxgun-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Frontier Tech
- Drones
- UAV
- Agriculture
- Robotics
- Agricultural Technology
- Flight Control
- eVTOL
- Hardware
---
