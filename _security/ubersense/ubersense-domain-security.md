---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ubersense.com
  spf: true
hosts:
- host: ubersense.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ubersense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UberSense, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: UberSense
provider_slug: ubersense
slug: ubersense-domain-security
source_filename: ubersense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubersense.com\n  https: false\ndomains:\n- domain: ubersense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubersense/refs/heads/main/security/ubersense-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Sports
- Video
- Coaching
- Mobile
- Acquired
---
