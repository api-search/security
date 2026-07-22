---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: happs.co
  spf: true
hosts:
- host: happs.co
  https: false
kind: domain-security
layout: security
method: probed
name: Happs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Happs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Happs
provider_slug: happs
slug: happs-domain-security
source_filename: happs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: happs.co\n  https: false\ndomains:\n- domain: happs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happs/refs/heads/main/security/happs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Live Streaming
- Video
- News
- Journalism
- Creator Economy
- Social Media
- Multistreaming
---
