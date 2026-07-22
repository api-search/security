---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 61draw.com
  spf: true
hosts:
- host: 61draw.com
  https: false
kind: domain-security
layout: security
method: probed
name: 61Draw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 61draw, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 61draw
provider_slug: 61draw
slug: 61draw-domain-security
source_filename: 61draw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 61draw.com\n  https: false\ndomains:\n- domain: 61draw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/61draw/refs/heads/main/security/61draw-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Education
- EdTech
- Online Learning
- Art
- Children
- Consumer
- China
---
