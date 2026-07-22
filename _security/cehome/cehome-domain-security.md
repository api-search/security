---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cehome.com
  spf: true
hosts:
- host: cehome.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cehome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cehome, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: cehome
provider_slug: cehome
slug: cehome-domain-security
source_filename: cehome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cehome.com\n  https: false\ndomains:\n- domain: cehome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cehome/refs/heads/main/security/cehome-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Construction Machinery
- Heavy Equipment
- Engineering Machinery
- Marketplace
- Used Equipment
- Community
- Industry News
- China
---
